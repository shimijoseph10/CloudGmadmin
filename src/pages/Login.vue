<template lang="html">

  <section class="login" style="padding-top:100px;">
    <div class="wrapper d-flex align-items-center auth login-full-bg">
      <div class="row w-100">
        <div class="col-lg-6 mx-auto">
          <div class="auth-form-dark text-left p-5">
            <h2>Login</h2>
            <h4 class="font-weight-light">Hello! let's get started</h4>
            <div v-if="err">
            <div>
              <b-alert show :duration="duration">{{err}}</b-alert>
            </div>
          </div>
            <form class="pt-5">
              <form @submit="onSubmit">
                <div class="form-group">
                  <label for="exampleInputEmail1">Username</label>
                  <input type="text" class="form-control" id="exampleInputEmail1"  required="" aria-describedby="emailHelp" placeholder="Username">
                  <i class="mdi mdi-account"></i>
                </div>
                <div class="form-group">
                  <label for="exampleInputPassword1">Password</label>
                  <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password"  required="">
                  <i class="mdi mdi-eye"></i>
                </div>
                <div class="mt-5">
                  <!-- <a class="btn btn-block btn-warning btn-lg font-weight-medium" href="../../index.html">Login</a> -->
                   <button type="submit" class="btn btn-success btn-lg btn-block">Sign In</button>
                </div>
                <div class="mt-3 text-center">
                  <a href="#" class="auth-link text-white">Forgot password?</a>
                </div>
              </form>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>

</template>


<style>
.main-panel {
    width: calc(100% - 0px);
    min-height: calc(100vh - 58px);
}
</style>
