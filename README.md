# Exercico-Sala-de-Aula-23-04
O useState é um Hook do React que permite criar e controlar estados dentro de componentes funcionais. Ele serve para armazenar valores que podem mudar ao longo do tempo, como textos, números, listas, etc.
import React, { useState } from "react";

function Contador() {
  const [contador, setContador] = useState(0);

  return (
    <div>
      <p>Valor: {contador}</p>
      <button onClick={() => setContador(contador + 1)}>
        Incrementar
      </button>
    </div>
  );
}

export default Contador;
O useEffect é um Hook usado para executar efeitos colaterais no componente.

Ele é utilizado para ações como:

Buscar dados de API
Manipular DOM
Executar algo quando o componente renderiza
import React, { useState, useEffect } from "react";

function ExemploEffect() {
  const [contador, setContador] = useState(0);

  useEffect(() => {
    console.log("O contador foi atualizado:", contador);
  }, [contador]);

  return (
    <div>
      <p>Valor: {contador}</p>
      <button onClick={() => setContador(contador + 1)}>
        Incrementar
      </button>
    </div>
  );
}

export default ExemploEffect;
