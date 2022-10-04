<template>
  <div class="container blog-header">
    <p class="h2">{{ user.name}}</p>
    <form class="form-inline form-search">
          <dl class="row">
            <dt class="col-sm-3"> User ID</dt>
            <dd class="col-sm-9">{{ user.id }}</dd>
            <dt class="col-sm-3"> Name - Lastname</dt>
            <dd class="col-sm-9">{{ user.name }} - {{ user.lastname }} </dd>
            <dt class="col-sm-3"> Email</dt>
            <dd class="col-sm-9">{{ user.email }} </dd>
            <dt class="col-sm-3"> Password</dt>
            <dd class="col-sm-9">{{ user.password }} </dd></dl>
    </form>
  </div>
</template>
<script>
import UserService from "@/services/UsersService";
export default {
  data() {
    return {
      user: null,
    };
  },
  async created() {
    try {
      let userId = this.$route.params.userId;
      this.user = (await UserService.show(userId)).data;
    } catch (error) {
      console.log(error);
    }
  },
};
</script>
<style scoped>
</style>