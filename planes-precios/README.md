    Tu página debe tener un elemento h1 con el texto Pricing Plans.
    Your page should have a div element with the class pricing-container below the h1 element.
        El selector .pricing-container debe tener una propiedad display con el valor flex y una propiedad flex-wrap con el valor wrap.
    Within the .pricing-container element, you should have three div elements with the class pricing-card to represent the pricing plans.
        Uno de los elementos .pricing-card debe tener la clase basic-plan además de la clase pricing-card.
        Uno de los elementos .pricing-card debe tener la clase pro-plan además de la clase pricing-card.
        Uno de los elementos .pricing-card debe tener la clase premium-plan además de la clase pricing-card.
    <!-- Tu elemento .basic-plan debe tener un elemento h2 con el texto Basic.
    Tu elemento .basic-plan debe tener un elemento p con el texto $9/month.
    Tu elemento .pro-plan debe tener un elemento h2 con el texto Pro.
    Tu elemento .pro-plan debe tener un elemento p con el texto $19/month. -->
    Tu elemento .premium-plan debe tener un elemento h2 con el texto Premium.
    Tu elemento .premium-plan debe tener un elemento p con el texto $29/month.
    Each of your .pricing-card elements should:
        Usa Flexbox para apilar su contenido en una columna y justificar el espacio entre los hijos usando space-between.
        Establece la propiedad flex en 0 0 200px para darle un ancho consistente y evitar que crezca o se reduzca en el diseño.
        Establece la propiedad border en 2px solid black para ver cómo las diferentes tarjetas ocupan espacio.
    El elemento .basic-plan debe aparecer primero en el diseño. Debes usar la propiedad order para esto.
    El elemento .pro-plan debe aparecer segundo en el diseño. Debes usar la propiedad order y establecer su propiedad flex-grow en 2 para que ocupe más espacio que los otros planes.
    El elemento .premium-plan debe ir al final del diseño. Debes usar la propiedad order para esto.

// ejecutando pruebas 5. Debes tener un selector .pricing-container. 6. Tu selector pricing-container debe tener la propiedad display con un valor de flex. 7. Tu selector .pricing-container debe tener la propiedad flex-wrap con un valor de wrap. 12. Debes tener un selector .pricing-card. 13. Tu selector .pricing-card debe tener la propiedad display con un valor de flex. 14. Tu selector .pricing-card debe tener la propiedad flex-direction con un valor de column. 15. Tu selector .pricing-card debe tener la propiedad justify-content con un valor de space-between. 16. Tu selector .pricing-card debe tener la propiedad flex con un valor de 0 0 200px. 17. Tu selector .pricing-card debe tener la propiedad border con un valor de 2px solid black. 18. Tu selector .basic-plan debe tener la propiedad order con un valor de 0. 23. Tu elemento .pro-plan debe tener la propiedad order con un valor de 1. 24. Tu elemento .pro-plan debe tener la propiedad flex-grow con un valor de 2. 27. Tu elemento premium-plan debe ser el último elemento en el diseño y tener la propiedad order con el valor 2.
// pruebas completadas

.pricing-container {
display: flex;
flex-wrap: wrap;
align-content: center;
border: 2px solid #000;
gap: 20px;
width: 80%;
max-width: 900px;
height: 70vh;
padding: 0 20px;
}

.pricing-card {
background: rgb(247, 247, 247);
box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
padding: 20px;
flex: 0 0 200px;
text-align: center;
transition: transform 0.3s ease;
display: flex;
flex-direction: column;
justify-content: space-between;
border: 2px solid black;
}
