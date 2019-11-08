<template>
  <div class="form">
    <div class="row">
      <div class="col s12">
        <h2>{{msg}}</h2>
      </div>
      <div class="col s4 leftpanel">
        <div class="row">
            <div class="input-field">
              <input value id="first_name2" type="text" class="validate" />
              <label class="active" for="first_name2">First Name</label>
            </div>
            <div class="input-field">
              <textarea id="textarea1" class="materialize-textarea"></textarea>
              <label for="textarea1">Textarea</label>
            </div>
            <div class="radiogroup">
              <label class="radiolbl">
                <input name="group1" type="radio" />
                <span>AWS</span>
              </label>

              <label class="radiolbl">
                <input name="group1" type="radio" />
                <span>Azure</span>
              </label>

              <label class="radiolbl">
                <input name="group1" type="radio" />
                <span>GCP</span>
              </label>
            </div>
        </div>
      </div>

      <div class="col s8 rightpanel">8-columns (one-half)</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Form",
  props: {
    msg: String
  }
};
</script>

<style scoped>
.leftpanel {
  padding-left: 2%;
}
.rightpanel {
  padding-right: 1%;
}
.radiogroup {
  padding-top: 5%;
  text-align: left;
}
.radiolbl{
    padding: 5%;
}
</style>