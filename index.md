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
</form>

<button onclick="gibslink()">Dă și mie</button>

<script>
  function gibslink() {
    let hasEiais = document.getElementById('eiais').checked
    let hasGi = document.getElementById('gi').checked
    let hasPi = document.getElementById('pi').checked
    let hasPsiho = document.getElementById('ppp').checked
    
    console.log(hasEiais, hasGi, hasPi, hasPsiho)

    if (!hasEiais && !hasGi && !hasPi) {
        window.alert('EROARE FATALA!! NU AI SELECTAT UN OPTIONAL')
        return
    }
    
    var link = 'https://serbuvlad.github.io/orare/312AA/orar'
    if (hasEiais)
        link += '_eiais'
    else if (hasGi)
        link += '_gi'
    else if (hasPi)
        link += '_pi'

    if (hasPsiho)
        link += '_psiho'

    link += '.xlsx'
    window.open(link)
  }
</script>
