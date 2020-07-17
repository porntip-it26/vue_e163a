
<template>

  <form>
    <v-text-field
      v-model="Username"
      :error-messages="UsernameErrors"
      :counter="10"
      label="Username"
      required
      @input="$v.Username.$touch()"
      @blur="$v.Username.$touch()"
    ></v-text-field>
    <v-text-field
      v-model="email"
      :error-messages="emailErrors"
      label="E-mail"
      required
      @input="$v.email.$touch()"
      @blur="$v.email.$touch()"
    ></v-text-field>
    <v-select
      v-model="Password"
      :items="Password"
      :error-messages="PasswordErrors"
      label="Password"
      required
      @change="$v.Password.$touch()"
      @blur="$v.Password.$touch()"
    ></v-select>
    <v-select
      v-model="Address"
      :items="Address"
      :error-messages="addressErrors"
      label="Address"
      required
      @change="$v.Address.$touch()"
      @blur="$v.Address.$touch()"
    ></v-select>
    <v-checkbox
      v-model="checkbox"
      :error-messages="checkboxErrors"
      label="Do you agree?"
      required
      @change="$v.checkbox.$touch()"
      @blur="$v.checkbox.$touch()"
    ></v-checkbox>

    <v-btn class="mr-4" @click="submit">ตกลง</v-btn>
    <nuxt-link to="/#/"><v-btn @click="clear">กลับหน้าแรก</v-btn></v-tab></nuxt-link>
  </form>
</template>