<template>
  <div class="maincontainer">
    <div class="contactinfo">
      <h4>Contact</h4>
      <p>3560 Lummen</p>
      <p>Belgium</p>
      <p>E-mail: Stef.wouters22@gmail.com</p>

    </div>
    <div class="formcontainer">
      <form data-netlify="true" method="post" id="idform" class="contactform" action="./contact" netlify>
        <div class="inputcontainer">
          <div class="namecontainer">
            <div class="fname">
              <label for="fname">First Name</label>
              <input type="text" id="fname" name="firstname" placeholder="Your name.." required>
            </div>
            <div class="lname">
              <label for="lname">Last Name</label>
              <input type="text" id="lname" name="lastname" placeholder="Your last name.." required>
            </div>
          </div>
          <div class="mailcontainer">
            <div class="mail">
              <label for="iemail">E-mail</label>
              <input type="email" id="iemail" name="e-mail" placeholder="Your e-mail.."
                     pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,4}$"
                     title="Please enter a correct email address" required>
            </div>
            <div class="phone">
              <label for="phone">Phone</label>
              <input type="tel" id="phone" name="phone" placeholder="Your phone number.."
                     pattern="[0-9]{10}"
                     required>
            </div>
          </div>
        </div>
        <div class="subjectbox">
          <label for="subject">Subject</label>
          <textarea id="subject" name="subject" placeholder="Write something.."></textarea>
        </div>

        <input class="sendbtn" type="submit" value="Submit">


      </form>
    </div>

  </div>
</template>

<script>
export default {
  name: "ContactView"
}
</script>

<style scoped>

.maincontainer {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-content: center;
  min-height: 84vh;
  max-height: 84vh;
}

.contactinfo {
  display: flex;
  flex-direction: column;
  justify-content: center;
  flex-wrap: wrap;
  padding-right: 4rem;
  margin-top: 10rem;
  float: left;
  border-right: 2px solid #42b983;
  margin-bottom: 8%;
}

.contactinfo p {
  color: var(--secondary-color);
  letter-spacing: 2px;
  word-spacing: 5px;
  line-height: 1.5rem;
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: center;
}

.contactinfo h4 {
  color: #42b983;
  font-size: 36px;
  letter-spacing: 2px;
  word-spacing: 5px;
  display: flex;
  flex-direction: row;
  float: left;
  justify-content: center;
}

.contactform {
  width: 50%;
  height: 40em;
  max-height: 50em;
  margin-top: 5rem;
  color: var(--secondary-color);
  padding-left: 4rem;
  display: flex;
  flex-direction: column;
  text-align: center;
  align-items: center;
  flex-wrap: wrap;
  float: right;
}

.formcontainer {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.fname {
  float: left;
  margin: 20px auto;
  padding-right: 1%;
}

.lname {
  float: right;
  margin: 20px auto;
  padding-left: 1%;
}

.namecontainer {
  align-content: center;
  display: flex;
  justify-content: space-between;
}

.inputcontainer {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
}

.contactform input[type="text"], .contactform input[type="email"] {
  background: none;
  border: 2px solid var(--secondary-color);
  padding: 10px 25px 15px;
  border-radius: 8px;
  outline: none;
  color: var(--secondary-color);

}

#phone {
  background: none;
  border: 2px solid var(--secondary-color);
  padding: 10px 25px 15px;
  border-radius: 8px;
  outline: none;
  color: var(--secondary-color);

}

#phone:focus {
  border-color: #42b983;
}

.contactform input[type = "text"]:focus, .contactform input[type="email"]:focus {
  border-color: #42b983;
}

.mailcontainer {
  align-content: center;
  display: flex;
  width: auto;
  justify-content: center;
}

.mail {
  float: left;
  margin: 20px;
  padding-right: 1%;
}

.phone {
  float: right;
  margin: 20px;
  padding-right: 1%;
}

.subjectbox {
  display: flex;
  justify-content: center;
  flex-direction: column;
}

#subject:focus {
  outline: none;
  border-color: #42b983;
  border-width: 2px;
}

#subject {
  width: 40em;
  height: 20em;
  margin-top: 3%;
  margin-bottom: 3%;
  background-color: var(--primary-color);
  color: var(--secondary-color);
  border-color: var(--secondary-color);
  border-width: 2px;
  border-radius: 6px;
}

textarea {
  resize: none;
}

.sendbtn {
  background: #42b983;
  color: var(--secondary-color);
  letter-spacing: 2px;
  border: none;
  border-radius: 8px;
  outline: none;
  width: 80px;
  height: 40px;
  box-shadow: inset 0 0 0 0 #2f8d62;
  transition: ease-in-out 0.5s;

}

.sendbtn:hover {
  box-shadow: inset 300px 0 0 0 #0cbf6c;
  cursor: pointer;
}
</style>