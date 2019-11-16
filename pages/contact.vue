<template>
  <v-container>
    <no-ssr>
      <form name="contact" method="post" action="" data-netlify="true" data-netlify-honeypot="bot-field">
        <v-text-field
          v-model="name"
          :error-messages="nameErrors"
          label="お名前*"
          required
          @input="$v.name.$touch()"
          @blur="$v.name.$touch()"
        ></v-text-field>
        <v-text-field
          v-model="email"
          :error-messages="emailErrors"
          label="メールアドレス*"
          required
          @input="$v.email.$touch()"
          @blur="$v.email.$touch()"
        ></v-text-field>
        <v-textarea
          v-model="message"
          :error-messages="messageErrors"
          label="メッセージ内容*"
          required
          @input="$v.message.$touch()"
          @blur="$v.message.$touch()"
          style="margin-bottom: 30px;"
        ></v-textarea>
        <v-btn type="submit" style="margin-bottom: 70px;">送信</v-btn>
      </form>
    </no-ssr>
  </v-container>
</template>

<script>
  import {validationMixin} from 'vuelidate'
  import {required, email} from 'vuelidate/lib/validators'

  export default {
    layout: 'layout',
    mixins: [validationMixin],

    validations: {
      name: {required},
      email: {required, email},
      message: {required}
    },

    data: () => ({
      name: '',
      email: '',
      message: '',
    }),
    computed: {
      messageErrors() {
        const errors = [];
        if (!this.$v.message.$dirty) return errors;
        !this.$v.message.required && errors.push('未入力です');
        return errors;
      },
      nameErrors() {
        const errors = [];
        if (!this.$v.name.$dirty) return errors;
        !this.$v.name.required && errors.push('未入力です');
        return errors;
      },
      emailErrors() {
        const errors = [];
        if (!this.$v.email.$dirty) return errors;
        !this.$v.email.email && errors.push('不正な値です');
        !this.$v.email.required && errors.push('未入力です');
        return errors;
      },
    },
  }
</script>
