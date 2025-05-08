
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Devis Photovoltaïque - Énergie Solaire</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; background: #f9f9f9; color: #333; }
    header { background: #33cc33; padding: 20px; color: white; text-align: center; }
    section { padding: 40px 20px; max-width: 800px; margin: auto; background: white; margin-top: 20px; border-radius: 10px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); }
    h1, h2 { text-align: center; }
    label { display: block; margin-top: 15px; font-weight: bold; }
    input, select { width: 100%; padding: 10px; margin-top: 5px; border-radius: 5px; border: 1px solid #ccc; }
    button { background: #33cc33; color: white; padding: 15px; border: none; border-radius: 5px; cursor: pointer; width: 100%; margin-top: 20px; }
    button:hover { background: #28a828; }
    iframe { border: 0; width: 100%; height: 600px; margin-top: 40px; border-radius: 10px; }
  </style>
</head>
<body>
  <header>
    <h1>Obtenez votre Devis Photovoltaïque</h1>
    <p>Profitez de l’énergie solaire dans le 67 et 57 🌞</p>
  </header>

  <section>
    <h2>Pourquoi passer au solaire ?</h2>
    <p>Réduisez votre facture d’électricité, valorisez votre bien immobilier et faites un geste pour la planète. Nos experts locaux vous accompagnent dans votre projet d’autoconsommation solaire.</p>
  </section>

  <section>
    <h2>Demande de devis</h2>
    <form id="quoteForm">
      <label for="name">Nom complet :</label>
      <input type="text" id="name" name="name" required />

      <label for="phone">Téléphone :</label>
      <input type="tel" id="phone" name="phone" required />

      <label for="email">Email :</label>
      <input type="email" id="email" name="email" required />

      <label for="codePostal">Code Postal (67 ou 57 uniquement) :</label>
      <input type="text" id="codePostal" name="codePostal" required pattern="^67\d{3}|57\d{3}$" />

      <label for="facture">Facture mensuelle (€) :</label>
      <input type="number" id="facture" name="facture" required />

      <label for="toiture">Type de toiture :</label>
      <select id="toiture" name="toiture" required>
        <option value="Tuile">Tuile</option>
        <option value="Ardoise">Ardoise</option>
        <option value="Tôle">Tôle</option>
        <option value="Autre">Autre</option>
      </select>

      <button type="submit">Envoyer ma demande</button>
    </form>
  </section>

  <section>
    <h2>Prendre rendez-vous avec un conseiller</h2>
    <p>Choisissez un créneau directement en ligne :</p>
    <iframe src="https://calendly.com/votre-lien" title="Prise de rendez-vous"></iframe>
  </section>

  <script>
    document.getElementById("quoteForm").addEventListener("submit", function(event) {
      event.preventDefault();

      const data = {
        name: document.getElementById("name").value,
        phone: document.getElementById("phone").value,
        email: document.getElementById("email").value,
        codePostal: document.getElementById("codePostal").value,
        facture: document.getElementById("facture").value,
        toiture: document.getElementById("toiture").value
      };

      fetch(https://script.google.com/macros/s/AKfycbx4RUSF30OfcJKzYPULN0YoWtjRILbc67hVcG4Rlfu44N5IatZWj5I39bjFHMwacroA0w/exec)://script.google.com/macros/s/exec", {
        method: "POST",
        body: JSON.stringify(data)
      })
      .then(res => alert("✅ Merci, votre demande a bien été envoyée."))
      .catch(err => alert("❌ Une erreur est survenue."));
    });
  </script>
</body>
</html>
