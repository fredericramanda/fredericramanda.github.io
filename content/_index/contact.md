+++
fragment = "contact"
#disabled = true
date = "2017-09-10"
weight = 1100
#background = "light"
form_name = "defaultContact"

title = "Formulaire de contact"
subtitle  = "*Remplissez ce formulaire pour nous contacter:*"

# PostURL can be used with backends such as mailout from caddy
post_url = "https://formspree.io/f/xoqpgnpl" #default: formspree.io
email = "fredericramanda@gmail.com"
button = "Envoyer" # defaults to theme default
#netlify = false

# Optional google captcha
#[recaptcha]
#  sitekey = ""

[message]
  #success = "" # defaults to theme default
  #error = "" # defaults to theme default

# Only defined fields are shown in contact form
[fields.name]
  text = "Votre Nom *"
  #error = "" # defaults to theme default

[fields.email]
  text = "Votre Email *"
  #error = "" # defaults to theme default

[fields.phone]
  text = "Votre Téléphone *"
  #error = "" # defaults to theme default

[fields.message]
  text = "Laissez nous un message *"
  #error = "" # defaults to theme default

# Optional hidden form fields
# Fields "page" and "site" will be autofilled
[[fields.hidden]]
  name = "page"

[[fields.hidden]]
  name = "site"

[[fields.custom]]
  name = "produit"
  text = "saisir le nom de solution qui vous intéresse: yzyhrm, vitalis, yzydistro"
  required = false
+++
