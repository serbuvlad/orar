# Orar 312AA

Orare mai ca lumea pentru 312AA.

<h2>Download</h2>
<form id="fform">
  <h4>Opționale:</h4>
  <input type="radio" name="opp" id="eiais">
  <label for="eiais">Elemente de Informatică Aplicate în Ingineria Sistemelor</label>
  <br>
  <input type="radio" name="opp" id="gi">
  <label for="eiais">Grafică Inginerească</label>
  <br>
  <input type="radio" name="opp" id="pi">
  <label for="eiais">Prelucrarea Informației</label>
  <br>
  <input type="checkbox" name="ppp" id="ppp">
  <label for="ppp">Psihologia Educației</label>
  <br>
  <button onclick="gibslink()">Dă link</button>
</form>

<script>
  function gibslink() {
    let form = document.getElementById('fform');
    let opt = form.elements['opp']
    let psih = form.elements['ppp']
    console.log(opt)
    console.log(psih)
  }
</script>
