<template>
  <v-form
    name="contact" netlify
    lazy-validation
  >
    <v-text-field
      name="name"
      :counter="10"
      label="Name"
      required
    ></v-text-field>

    <v-text-field
      email="email"
      label="E-mail"
      required
    ></v-text-field>

  
    <v-btn
      color="warning"
      type="submit"
    >
      Submit
    </v-btn>
  </v-form>
</template>

