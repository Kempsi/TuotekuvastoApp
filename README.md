# TuotekuvastoApp

## Sovelluksen kuvaus

### HomeController.cs
#### Tämä on sovelluksen päälogiikka, mikä ohjaa tuotteiden sivulle ja sieltä hakee json-tiedoston sisällön.
#### Product() - metod kutsuu GetProducts() - metodia, joka lukee products.jsonin ja muuntaa sen Product ilmentymiksi. Palauttaa tuotetiedot Product.cshtml näkymään

### Products.json
#### Sisältää tuotteiden tiedot.
#### HomeController käyttää tätä tuotteiden varastona ja lukee sen GetProduct() - metodilla.

### Product.cs 
#### Malliluokka, mikä määrittelee tuotteen rakenteen. 

### Product.cshtml
#### Näkymä, joka näyttää tuotteet käyttöliittymässä. Käyttää Product.cs malliluokkaa.
#### Luo liston Product ilmentymiä käyttöliittymään.

### Yhteistoiminta
#### HomeController.cs hakee tuotetiedot json tiedostosta, deserialisoi ne ja vie sen Product.csthml näkymään
#### Product.cshtml käyttää Product.cs malliluokkaa ja näyttää ne käyttäjälle
