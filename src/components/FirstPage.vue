
<template>
 <div className="container-scroller">
        <div className="container-fluid page-body-wrapper full-page-wrapper">
          <div className="content-wrapper d-flex align-items-center auth login-full-bg">
            <div className="row w-100 margin-l-0">
              <div className="col-lg-4 mx-auto">
                <div className="auth-form-light text-left p-5">
                  <div className="login-header">
                    <!-- <img src="../assets/images/logo.png" /> -->
                    <hr />
                    <h4 className="font-weight-light">Admin Login</h4>
                  </div>
                  <form className="pt-5" autoComplete="off" onSubmit={this.login}>
                    <div className="form-group">
                      <input className="form-control" type="text" name="email" placeholder="Enter Email" pattern="^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$" onChange={this.handleChange}/>
                      <i className="fa fa-user" aria-hidden="true" />
                    </div>
                    <div className="form-group">
                      <input className="form-control" type="password" name="password" placeholder="Enter Password" id="password" required onChange={this.handleChange}/>
                      <i className="fa fa-lock" aria-hidden="true" />
                    </div>
                    <div className="mt-5">
                      <button className="btn btn-block btn-primary btn-lg font-weight-medium" type="submit">Login</button>
                    </div>
                    <div className="row">
                      <div className="col-md-6 col-sm-6">
                        <div className="form-check">
                          <label className="form-check-label">
                            <input type="checkbox" className="form-check-input" name="rememberMe"  onClick={this.saveUser.bind(this)}/>
                            Remember Password
                            <i className="input-helper" /></label>
                        </div> 
                      </div>
                      <div className="col-md-6 col-sm-6">
                        <div className="mt-3 text-right">
                          <a onClick={this.showForgotPassword} className="auth-link text-gray" >Forgot password?</a>
                        </div>
                      </div>
                    </div>
                  </form>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
</template>

<script>
import { mapState, mapActions } from "vuex";
export default {
  name: "FirstPage",
  components: {},
  data: () => ({
    message: "Welcome to Your Vue.js App",
    message1: "go and have a life",
    message2: "Yeah i will look for it"
  }),
  computed: {},
  methods: {}
};
</script>

<style src="../../static/css/style.css">
</style>

