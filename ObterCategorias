// Simulando postagens associadas a marcadores
const postagensPorMarcador = {
    tecnologia: [
        { titulo: 'Postagem sobre tecnologia 1', conteudo: 'Conteúdo da postagem 1...' },
        { titulo: 'Postagem sobre tecnologia 2', conteudo: 'Conteúdo da postagem 2...' }
    ],
    viagem: [
        { titulo: 'Postagem sobre viagem 1', conteudo: 'Conteúdo da postagem 1...' },
        { titulo: 'Postagem sobre viagem 2', conteudo: 'Conteúdo da postagem 2...' }
    ],
    culinaria: [
        { titulo: 'Postagem sobre culinária 1', conteudo: 'Conteúdo da postagem 1...' },
        { titulo: 'Postagem sobre culinária 2', conteudo: 'Conteúdo da postagem 2...' }
    ]
};

// Função para atualizar as postagens exibidas com base no marcador selecionado
function atualizarPostagens() {
    const marcadorDropdown = document.getElementById('marcadorDropdown');
    const postagensContainer = document.getElementById('postagens');
    const marcadorSelecionado = marcadorDropdown.value;

    // Limpar as postagens exibidas anteriormente
    postagensContainer.innerHTML = '';

    // Exibir as postagens associadas ao marcador selecionado
    const postagens = postagensPorMarcador[marcadorSelecionado];
    postagens.forEach(postagem => {
        const postagemElement = document.createElement('div');
        postagemElement.innerHTML = `<h2>${postagem.titulo}</h2><p>${postagem.conteudo}</p>`;
        postagensContainer.appendChild(postagemElement);
    });
}

// Associar a função ao evento de mudança no menu suspenso
const marcadorDropdown = document.getElementById('marcadorDropdown');
marcadorDropdown.addEventListener('change', atualizarPostagens);

// Exibir postagens iniciais ao carregar a página
atualizarPostagens();
