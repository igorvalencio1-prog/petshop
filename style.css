// ==============================
// DATA E HORA ATUAL
// ==============================

function mostrarDataAtual() {
    const elemento = document.getElementById("dataAtual");

    if (elemento) {
        const agora = new Date();

        const data = agora.toLocaleDateString("pt-BR");
        const hora = agora.toLocaleTimeString("pt-BR");

        elemento.textContent =
            "Data e hora atual: " + data + " - " + hora;
    }
}

mostrarDataAtual();


// ==============================
// CARROSSEL
// ==============================

let imagemAtual = 0;

function mostrarImagem(numero) {

    const imagens = document.querySelectorAll(".imagem-carrossel");

    if (imagens.length === 0) {
        return;
    }

    imagens.forEach(function(imagem) {
        imagem.style.display = "none";
    });

    imagemAtual = numero;

    if (imagemAtual >= imagens.length) {
        imagemAtual = 0;
    }

    if (imagemAtual < 0) {
        imagemAtual = imagens.length - 1;
    }

    imagens[imagemAtual].style.display = "block";
}


function proximaImagem() {
    mostrarImagem(imagemAtual + 1);
}


function imagemAnterior() {
    mostrarImagem(imagemAtual - 1);
}


mostrarImagem(0);


// ==============================
// FORMULÁRIO DE AGENDAMENTO
// ==============================

const formulario = document.querySelector("form");

if (formulario) {

    formulario.addEventListener("submit", function(evento) {

        evento.preventDefault();

        const nome = document.getElementById("nome");
        const pet = document.getElementById("pet");
        const servico = document.getElementById("servico");
        const data = document.getElementById("data");
        const horario = document.getElementById("horario");

        if (
            nome &&
            pet &&
            servico &&
            data &&
            horario
        ) {

            alert(
                "Agendamento realizado com sucesso!\n\n" +
                "Cliente: " + nome.value + "\n" +
                "Pet: " + pet.value + "\n" +
                "Serviço: " + servico.value + "\n" +
                "Data: " + data.value + "\n" +
                "Horário: " + horario.value
            );

            formulario.reset();
        }

    });

}
