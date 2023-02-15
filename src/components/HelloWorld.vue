<template>
  <div class="input-page">
    <h1>Wedding Information</h1>
    <form>
      <h2>Groom Information</h2>
      <div class="form-group">
        <label for="groomName">Groom Name:</label>
        <input type="text" id="groomName" v-model="groomName" required>
      </div>
      <div class="form-group">
        <label for="groomFather">Groom Father:</label>
        <input type="text" id="groomFather" v-model="groomFather" required>
      </div>
      <div class="form-group">
        <label for="groomMother">Groom Mother:</label>
        <input type="text" id="groomMother" v-model="groomMother" required>
      </div>
      <div class="form-group">
        <label for="groomRelation">Groom Relation:</label>
        <input type="text" id="groomRelation" v-model="groomRelation" required>
      </div>
      <div class="form-group">
        <label for="groomPhone">Groom Phone:</label>
        <input type="tel" id="groomPhone" v-model="groomPhone" required>
      </div>
      <div class="form-group">
        <label for="groomBank">Groom Bank:</label>
        <input type="text" id="groomBank" v-model="groomBank" required>
      </div>
      <div class="form-group">
        <label for="groomAccountOwn">Groom Account Owner:</label>
        <input type="text" id="groomAccountOwn" v-model="groomAccountOwn" required>
      </div>
      <div class="form-group">
        <label for="groomAccountNum">Groom Account Number:</label>
        <input type="text" id="groomAccountNum" v-model="groomAccountNum" required>
      </div>
      <h2>Bride Information</h2>
      <div class="form-group">
        <label for="brideName">Bride Name:</label>
        <input type="text" id="brideName" v-model="brideName" required>
      </div>
      <div class="form-group">
        <label for="brideFather">Bride Father:</label>
        <input type="text" id="brideFather" v-model="brideFather" required>
      </div>
      <div class="form-group">
        <label for="brideMother">Bride Mother:</label>
        <input type="text" id="brideMother" v-model="brideMother" required>
      </div>
      <div class="form-group">
        <label for="brideRelation">Bride Relation:</label>
        <input type="text" id="brideRelation" v-model="brideRelation" required>
      </div>
      <div class="form-group">
        <label for="bridePhone">Bride Phone:</label>
        <input type="tel" id="bridePhone" v-model="bridePhone" required>
      </div>
      <div class="form-group">
        <label for="brideBank">Bride Bank:</label>
        <input type="text" id="brideBank" v-model="brideBank" required>
      </div>
      </div>
      <div class="form-group">
          <label for="brideAccountOwn">Bride Account Owner:</label>
    <input type="text" id="brideAccountOwn" v-model="brideAccountOwn" required>
  </div>

  <div class="form-group">
    <label for="brideAccountNum">Bride Account Number:</label>
    <input type="text" id="brideAccountNum" v-model="brideAccountNum" required>
  </div>

  <h2>Wedding Details</h2>
  <div class="form-group">
    <label for="weddingHall">Wedding Hall:</label>
    <input type="text" id="weddingHall" v-model="weddingHall" required>
  </div>
  <div class="form-group">
    <label for="detailAddress">Detail Address:</label>
    <input type="text" id="detailAddress" v-model="detailAddress" required>
  </div>

      <div class="form-group">
        <h2>Wedding Details</h2>

        <label for="weddingHall">Hall</label>
        <input type="text" id="weddingHall" v-model="weddingHall" required>

        <label for="detailAddress">Detail Address</label>
        <textarea id="detailAddress" v-model="detailAddress" required></textarea>

        <label for="address">Address</label>
        <input type="text" id="address" v-model="address" required>

        <label for="weddingDate">Date</label>
        <input type="date" id="weddingDate" v-model="weddingDate" required>

        <label for="greetingsTitle">Greetings Title</label>
        <input type="text" id="greetingsTitle" v-model="greetingsTitle" required>

        <label for="greetingsBody">Greetings Body</label>
        <textarea id="greetingsBody" v-model="greetingsBody" required></textarea>

        <label for="text">Text</label>
        <textarea id="text" v-model="text" required></textarea>

        <label for="notice">Notice</label>
        <textarea id="notice" v-model="notice" required></textarea>
      </div>

      <button type="submit">Submit</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      groomName: '',
      groomFather: '',
      groomMother: '',
      groomRelation: '',
      groomPhone: '',
      groomBank: '',
      groomAccountOwn: '',
      groomAccountNum: '',
      brideName: '',
      brideFather: '',
      brideMother: '',
      brideRelation: '',
      bridePhone: '',
      brideBank: '',
      brideAccountOwn: '',
      brideAccountNum: '',
      weddingHall: '',
      detailAddress: '',
      address: '',
      weddingDate: '',
      greetingsTitle: '',
      greetingsBody: '',
      text: '',
      notice: ''
    };
  },
  methods: {
    submitForm() {
      // submit the form data to the server-side script for processing
      console.log('Form data submitted:', this.$data);
      // clear the form fields after submission
      Object.assign(this.$data, this.$options.data());
    }
  }
};
</script>

<style>
  .input-page {
    max-width: 600px;
    margin: 0 auto;
  }

  h1, h2 {
    text-align: center;
  }

  .form-group {
    margin-bottom: 1rem;
  }

  label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: bold;
  }

  input, textarea {
    width: 100%;
    padding: 0.5rem;
    border-radius: 5px;
    border: 


<style>
  .input-page {
    max-width: 600px;
    margin: 0 auto;
    font-family: Arial, sans-serif;
    color: #333;
  }

  h1, h2 {
    text-align: center;
    margin-top: 2rem;
    margin-bottom: 1rem;
  }

  .form-group {
    margin-bottom: 1rem;
  }

  label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: bold;
  }

  input, textarea {
    width: 100%;
    padding: 0.5rem;
    border-radius: 5px;
    border: 1px solid #ccc;
    box-sizing: border-box;
    font-size: 1rem;
  }

  input:focus, textarea:focus {
    outline: none;
    border-color: #8a3ffc;
  }

  button[type="submit"] {
    display: block;
    margin-top: 2rem;
    padding: 0.5rem;
    background-color: #8a3ffc;
    color: #fff;
    border: none;
    border-radius: 5px;
    font-size: 1rem;
    cursor: pointer;
  }

  button[type="submit"]:hover {
    background-color: #6c2dcb;
  }
</style>