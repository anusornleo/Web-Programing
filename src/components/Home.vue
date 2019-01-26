<!-- src/components/Home.vue -->
<template>
  <div class="bg_login">
    <div class="harf_bg">
      <h1>Sign in</h1>
      <form action="main.vue" class="center_login">
        <input type="email" id="email" name="email" placeholder="Email">
        <input type="password" id="password" name="password" placeholder="Password">
        <input type="submit" value="Login" @click="gomain">
      </form>
      <button type="button" class="btn btn-default btn-lg" @click="goAdd">
      <span class="glyphicon glyphicon-plus" aria-hidden="true" ></span> Add
    </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  methods: {
    goAdd: function() {
      this.$router.push("/main");
    }
  }
};
</script>

<style scoped>
.bg_login{
  background-color: #00897b;
  width: 100%;
  height: -webkit-fill-available;
}
.harf_bg {
  background-color: white;
  position: absolute;
  top: 0px;
  left: 50%;
  width: 50%;
  height: -webkit-fill-available;
}

/* input username or password CSS */

h1 {
  text-align: center;
  padding: 12% 0px 0px 3%;
}

input[type="email"] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 3px solid #ccc;
  -webkit-transition: 0.5s;
  transition: 0.5s;
  outline: none;
  border-radius: 24px;
}

input[type="password"] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 3px solid #ccc;
  -webkit-transition: 0.5s;
  transition: 0.5s;
  outline: none;
  border-radius: 24px;
}

input[type="submit"] {
  width: 30%;
  background-color: #b2dfdb;
  color: rgb(255, 255, 255);
  padding: 13px 20px;
  margin: 8px 35%;
  border: none;
  border-radius: 24px;
  cursor: pointer;
  -webkit-transition: 0.5s;
  transition: 0.5s;
}

input[type="email"]:focus {
  border: 3px solid #555;
}

input[type="password"]:focus {
  border: 3px solid #555;
}

input[type="submit"]:hover {
  background-color: #00897b;
  color: rgb(255, 255, 255);
}

.center_login {
  position: absolute;
  margin: 4% 0 0 27%;
  width: 50%;
}
</style>