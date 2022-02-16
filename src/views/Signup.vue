<template>
  <div class="signup bg-ljubicasta text-roza">
    <h1 class="text-white">This is a signup page</h1>
    <div class="container">
      <div class="row">
        <div class="col-sm"></div>
        <div class="col-sm">
          <form
            oninput='confirmPassword.setCustomValidity(confirmPassword.value != passwordInput.value ? "Passwords do not match." : "")'
          >
            <div class="form-group">
              <label for="nameInput">Name</label>
              <input
                type="text"
                class="form-control"
                id="nameInput"
                placeholder="Enter name"
              />
            </div>
            <div class="form-group">
              <label for="lastNameInput">Last name</label>
              <input
                type="text"
                class="form-control"
                id="lastNameInput"
                placeholder="Enter lastname"
              />
            </div>
            <div class="form-group">
              <label for="usernameInput">Preferred username</label>
              <input
                type="text"
                class="form-control"
                id="usernameInput"
                placeholder="Enter lastname"
              />
            </div>
            <div class="form-group">
              <label for="emailInput">Email address</label>
              <input
                type="email"
                class="form-control"
                id="emailInput"
                aria-describedby="emailHelp"
                placeholder="Enter email"
              />
              <small id="emailHelp" class="form-text text-muted"
                >We'll never share your email with anyone else.</small
              >
            </div>
            <div class="form-group">
              <label for="passwordInput">Password</label>
              <input
                type="password"
                class="form-control"
                id="passwordInput"
                placeholder="Password"
              />
            </div>
            <div class="form-group">
              <label for="confirmPassword">Confirm password</label>
              <input
                type="password"
                class="form-control"
                id="confirmPassword"
                placeholder="Confirm password"
              />
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
          </form>
        </div>
        <div class="col-sm"></div>
      </div>
    </div>
  </div>
</template>
