---
enable: true # Control the visibility of this section across all pages where it is used
title: "Have Any Project on Your Mind?"
description: "Great! We're excited to hear from you and let's start something"

# image: "/images/about-us/about-one.jpg"
# imagePosition: "left" # Choose between "left" or "right"

map:
  enable: true
  position: "right" # Choose between "left" or "right"
  title: "Map of New Work City"
  url: https://maps.google.com/maps?width=100%25&amp;height=600&amp;hl=en&amp;q=1%20Grafton%20Street,%20Dublin,%20Ireland+(My%20Business%20Name)&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed # Embed map iframe URL generated from https://www.maps.ie/create-google-map/

# contactInformation:
#   - title: "Headquarters"
#     icon: "/images/icons/svg/location-filled.svg"
#     description: "27 Division St, New York, NY 10002, USA"
#     button:
#       # Refer to the `sharedButton` schema in `src/sections.schema.ts` for all available configuration options (e.g., enable, label, url, hoverEffect, variant, icon, tag, rel, class, target, etc.)
#       enable: true
#       label: "Get Direction"
#       url: "/"
#       # hoverEffect: "" # Optional: text-flip | creative-fill | magnetic | magnetic-text-flip
#       # variant: "" # Optional: fill | outline | text | circle
#       # rel: "" # Optional
#       # target: "" # Optional
#
#   - title: "Email Address"
#     icon: "/images/icons/svg/message-filled.svg"
#     description: |
#       folex.agency@mail.com
#       folex.agency@support.com
#     button:
#       # Refer to the `sharedButton` schema in `src/sections.schema.ts` for all available configuration options (e.g., enable, label, url, hoverEffect, variant, icon, tag, rel, class, target, etc.)
#       enable: true
#       label: "Send Message"
#       url: "mailto:folex.agency@mail.com"
#       # hoverEffect: "" # Optional: text-flip | creative-fill | magnetic | magnetic-text-flip
#       # variant: "" # Optional: fill | outline | text | circle
#       # rel: "" # Optional
#       # target: "" # Optional
#
#   - title: "Phone Number"
#     icon: "/images/icons/svg/phone-filled.svg"
#     description: |
#       +1 800 123 654 987
#       +1 800 223 984 002
#     button:
#       # Refer to the `sharedButton` schema in `src/sections.schema.ts` for all available configuration options (e.g., enable, label, url, hoverEffect, variant, icon, tag, rel, class, target, etc.)
#       enable: true
#       label: "Call Anytime"
#       url: "tel:+1800123654987"
#       # hoverEffect: "" # Optional: text-flip | creative-fill | magnetic | magnetic-text-flip
#       # variant: "" # Optional: fill | outline | text | circle
#       # rel: "" # Optional
#       # target: "" # Optional

# Check config.toml file for form action related settings
# this is also used in the footer of the personal portfolio homepage
form:
  emailSubject: "Nuevo mensaje desde el sitio Micrafil" # Customized email subject (applicable when anyone submit form, form submission may receive by email depend on provider)
  submitButton:
    # Refer to the `sharedButton` schema in `src/sections.schema.ts` for all available configuration options (e.g., enable, label, url, hoverEffect, variant, icon, tag, rel, class, target, etc.)
    enable: true
    label: "Enviar Mensaje"
    # hoverEffect: "" # Optional: text-flip | creative-fill | magnetic | magnetic-text-flip
    # variant: "" # Optional: fill | outline | text | circle
    # rel: "" # Optional
    # target: "" # Optional

  # This note will show at the end of form
  # note: |
  #   Your data is safe with us. We respect your privacy and never share your information. <br /> Read our [Privacy Policy](/privacy-policy/).
  inputs:
    - label: ""
      placeholder: "Nombre Completo *"
      name: "Nombre Completo" # This is crucial. Its indicate under which name you want to receive this field data
      required: true
      halfWidth: true
      defaultValue: ""
    - label: ""
      placeholder: "Correo Electrónico *"
      name: "Correo Electrónico" # This is crucial. Its indicate under which name you want to receive this field data
      required: true
      type: "email"
      halfWidth: true
      defaultValue: ""
    - label: ""
      placeholder: "Teléfono / WhatsApp *"
      name: "Teléfono"
      required: true
      type: "tel"
      halfWidth: true
      defaultValue: ""
    - label: ""
      placeholder: "Motivo *"
      name: "Motivo"
      required: true
      halfWidth: true
      dropdown:
        type: "" # select | search - default is select
        search: # if type is search then it will work
          placeholder: ""
        items:
          - label: "Hogar (Doméstico)"
            value: "Hogar (Doméstico)"
            selected: false
          - label: "Comercial"
            value: "Comercial"
            selected: false
          - label: "Hotelería / Restaurantes"
            value: "Hotelería / Restaurantes"
            selected: false
          - label: "Industrial"
            value: "Industrial"
            selected: false
    - label: ""
      placeholder: "Motivo específico"
      name: "Motivo Específico" # This is crucial. Its indicate under which name you want to receive this field data
      required: false
      halfWidth: true
      dropdown:
        type: "search" # select | search - default is select
        search: # if type is search then it will work
          placeholder: "Buscar solicitudes"
        items:
          - label: "Ósmosis Inversa"
            value: "Ósmosis Inversa"
            selected: false
          - label: "Ósmosis + UV"
            value: "Ósmosis + UV"
            selected: false
          - label: "Suavizador de Agua"
            value: "Suavizador de Agua"
            selected: false
          - label: "Sistema Industrial"
            value: "Sistema Industrial"
            selected: false
          - label: "Sistema para Restaurante / Café"
            value: "Sistema para Restaurante / Café"
            selected: false
          - label: "Desmineralización"
            value: "Desmineralización"
            selected: false
          - label: "Problemas de Incrustaciones"
            value: "Problemas de Incrustaciones"
            selected: false
          - label: "Mantenimiento"
            value: "Mantenimiento"
            selected: false
          - label: "Refacciones"
            value: "Refacciones"
            selected: false
          - label: "Análisis de Agua"
            value: "Análisis de Agua"
            selected: false
          - label: "Proyecto Especial"
            value: "Proyecto Especial"
            selected: false
    - label: ""
      tag: "textarea"
      defaultValue: ""
      rows: "2" # Only work if tag is textarea
      placeholder: "¿Cómo podemos ayudarte? *"
      name: "Mensaje" # This is crucial. Its indicate under which name you want to receive this field data
      required: true
      halfWidth: false
    - label: "Búsqueda en Google" # only valid for type="checkbox" & type === "radio"
      checked: false # only valid for type="checkbox" & type === "radio"
      name: "Origen del contacto" # This is crucial. Its indicate under which name you want to receive this field data
      required: true
      groupLabel: "¿Cómo te enteraste de nosotros?" # Radio Inputs Label
      group: "source" # when you add group then it will omit space between the same group radio input
      type: "radio"
      halfWidth: true
      defaultValue: ""
    - label: "Redes Sociales" # only valid for type="checkbox" & type === "radio"
      name: "Origen del contacto" # This is crucial. Its indicate under which name you want to receive this field data
      required: true
      groupLabel: "" # Radio Inputs Label
      group: "source" # when you add group then it will omit space between the same group radio input
      type: "radio"
      halfWidth: true
      defaultValue: ""
    - label: "Recomendación"
      name: "Origen del contacto"
      required: true
      groupLabel: ""
      group: "source"
      type: "radio"
      halfWidth: true
      defaultValue: ""
    - label: "Ya conozco Micrafil"
      name: "Origen del contacto"
      required: true
      groupLabel: ""
      group: "source"
      type: "radio"
      halfWidth: true
      defaultValue: ""
    - label: "Acepto los términos y condiciones y [aviso de privacidad](/)." # only valid for type="checkbox" & type === "radio"
      id: "privacy-policy"
      name: "Aceptación de Términos" # This is crucial. Its indicate under which name you want to receive this field data
      value: "Agreed" # Value that will be submit (applicable for type="checkbox" & type === "radio")
      checked: false # only valid for type="checkbox" & type === "radio"
      required: true
      type: "checkbox"
      halfWidth: false
      defaultValue: ""
    - note: success # info | warning | success | deprecated | hint
      parentClass: "hidden text-sm message success"
      content: ¡Hemos recibido tu mensaje! Te contactaremos lo antes posible.
    - note: deprecated # info | warning | success | deprecated | hint
      parentClass: "hidden text-sm message error"
      content: Algo salió mal. Escríbenos a [folex-astro-theme@gmail.com](mailto:folex-astro-theme@gmail.com) para recibir ayuda.
---
