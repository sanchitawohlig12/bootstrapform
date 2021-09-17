<template>
  <div>
    <v-sheet
      :elevation="elevation"
      class="mx-auto"
      height="550"
      :width="$vuetify.breakpoint.mdAndUp ? '450' : '380'"
    >
      <div class="div text-center pt-4" v-if="$vuetify.breakpoint.mdAndUp">
        <v-btn color="deep-orange" small dark> FILL IN YOUR DETAILS </v-btn>
      </div>
      <div class="div" v-if="$vuetify.breakpoint.smAndDown">
        <v-btn color="deep-orange" small dark> FILL IN YOUR DETAILS </v-btn>
      </div>

      <v-form class="form">
        <v-row>
          <v-col>
            <div class="inputWithIcon">
              <input type="text" placeholder="Enter Your Full name" />
              <i class="fa fa-user fa-fw" area-hidden="true"></i>
            </div>

            <div class="inputWithIcon1">
              <input type="text" placeholder=" Enter Email" />
              <i class="fa fa-envelope" area-hidden="true"></i>
            </div>

            <div class="inputWithIcon2">
              <input type="text" placeholder=" Enter Phone Number" />
              <i class="fa fa-phone fa-fw" area-hidden="true"></i>
            </div>
            <div class="inputWithIcon3">
              <input type="text" placeholder=" Enter Password" />
              <i class="fa fa-lock fa-fw" area-hidden="true"></i>
            </div>
          </v-col>
        </v-row>
        <div class="text-center">
          <v-btn color="deep-orange" small dark class="btn"> SUBMIT </v-btn>
        </div>
        <div class="main">
          <label for="exampleFormControlSelect1" class="label"
            >Which team will score the maximum boundaries this IPL?</label
          >
          <select class="form-control" id="exampleFormControlSelect1">
            <option>1</option>
            <option>2</option>
            <option>3</option>
            <option>4</option>
            <option>5</option>
          </select>
          <label for="exampleFormControlSelect1" class="label"
            >Which team will hit the maximum sixes this IPL?</label
          >
          <select class="form-control" id="exampleFormControlSelect1">
            <option>1</option>
            <option>2</option>
            <option>3</option>
            <option>4</option>
            <option>5</option>
          </select>
          <label for="exampleFormControlSelect1" class="label"
            >Which team will take the maximum wickets this IPL?</label
          >
          <select class="form-control" id="exampleFormControlSelect1">
            <option>1</option>
            <option>2</option>
            <option>3</option>
            <option>4</option>
            <option>5</option>
          </select>
          <label for="exampleFormControlSelect1" class="label"
            >Which team's player will be the Orange cap winner this IPL?</label
          >
          <select class="form-control" id="exampleFormControlSelect1">
            <option>1</option>
            <option>2</option>
            <option>3</option>
            <option>4</option>
            <option>5</option>
          </select>
          <label for="exampleFormControlSelect1" class="label"
            >Which team's player will be the Purple cap winner this IPL?</label
          >
          <select class="form-control" id="exampleFormControlSelect1">
            <option>1</option>
            <option>2</option>
            <option>3</option>
            <option>4</option>
            <option>5</option>
          </select>
        </div>
        <div class="footer">
          <h6 class="h6">Terms and Condition:</h6>
          <p>
            <i class="fa fa-circle"
              ><span class="span" style="color: black">Sign up</span></i
            >
             <i class="fa fa-circle"
              ><span class="span" style="color: black">Fill in your Fairplay details</span></i
            >
            <i class="fa fa-circle"
              ><span class="span" style="color: black ">Submit your answer</span></i
            >
            <i class="fa fa-circle"
              ><span class="span" style="color: black">Need to own a passport</span></i
            >
          </p>
        </div>
      </v-form>
    </v-sheet>
  </div>
</template>
<style scoped>
.form {
  width: 60%;
  margin-left: 35px;
  margin-top: 10px;
}
.mx-auto {
  background-image: linear-gradient(#c0c0c0, #808080);
  border-radius: 15px;
}
.btn {
  margin-left: 100px;
}
.form-control {
  border-radius: 40px !important;
  outline: none;
  height: 30px;
  width: 400px;
  font-size: 15px;
  margin-bottom: 10px;
}
.h6{
  font-weight:bold;
  padding-left:8px;
}
.inputWithIcon i {
  position: absolute;
  left: 590px;
  top: 75px;
}
.inputWithIcon1 i {
  position: absolute;
  left: 590px;
  top: 115px;
}
.inputWithIcon2 i {
  position: absolute;
  left: 590px;
  top: 155px;
}
.inputWithIcon3 i {
  position: absolute;
  left: 590px;
  top: 195px;
}
p i {
  color: red;
  padding-left:10px;
  font-size:13px;
  font-weight:normal;
  
}
.span {
  padding-left: 5px;
  font-family:'Arial';
  margin-bottom:20px;
}

input[type='text'] {
  padding-left: 30px;
  border-radius: 57px;
  background: white;

  width: 400px;
  height: 30px;
  margin-bottom: 10px;
  outline: none;
}
.footer {
  border: 1px solid black;
  border-radius: 10px;
  margin-top: 20px;
  height: 80px;
  width: 450px;
  margin-left:-33px;
  margin-top:30px;
}
.label {
  font-size: 13px;
  color: black;
}

@media only screen and (max-width: 991px) {
  .mx-auto {
    height: 300px;
    width: 30px;
  }
  .form {
    margin-left: 20px;
  }
  .div {
    padding-top: 20px;
    margin-left: 110px;
  }
  input[type='text'] {
    padding-left: 30px;
    border-radius: 57px;
    background: white;

    width: 350px;
    height: 30px;
    margin-bottom: 10px;
    outline: none;
  }
  .form-control {
    border-radius: 40px !important;
    outline: none;
    height: 30px;
    width: 350px;
    font-size: 15px;
  }
  .inputWithIcon i {
    position: absolute;
    left: 40px;
    top: 75px;
  }
  .inputWithIcon1 i {
    position: absolute;
    left: 40px;
    top: 115px;
  }
  .inputWithIcon2 i {
    position: absolute;
    left: 40px;
    top: 155px;
  }
  .inputWithIcon3 i {
    position: absolute;
    left: 40px;
    top: 195px;
  }
  .footer {
  border: 1px solid black;
  border-radius: 10px;
  margin-top: 20px;
  height: 80px;
  width: 380px;
  margin-left:-20px;
}
}
</style>