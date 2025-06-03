# Sistema de Senhas - ETEC Adolpho Arruda Mello

## Descrição

Este projeto é um sistema de gerenciamento e exibição de senhas de atendimento, desenvolvido para a ETEC Adolpho Arruda Mello. Ele permite chamar senhas normais e prioritárias, exibe a senha atual de forma destacada, mantém um histórico das últimas chamadas, mostra um relógio em tempo real e possui um espaço para a exibição de um vídeo institucional. A operação do sistema é realizada primariamente através de atalhos de teclado para agilidade.

## ✨ Funcionalidades

* **Chamada de Senhas:**
    * Senhas Normais (prefixo 'N')
    * Senhas Prioritárias (prefixo 'P')
* **Display Principal:** Exibição grande e clara da senha atual chamada.
* **Histórico de Chamadas:** Lista das últimas 5 senhas chamadas, com o respectivo horário (HH:MM).
* **Relógio Digital:** Exibição do horário atual (HH:MM:SS).
* **Vídeo Institucional:** Espaço dedicado para a reprodução de um vídeo em loop.
* **Controles por Teclado:** Operação ágil através de atalhos:
    * `N`: Chama a próxima senha normal.
    * `P`: Chama a próxima senha prioritária.
    * `Q`: Reinicia a contagem de todas as senhas e o histórico.
* **Feedback Sonoro:** Emissão de um som ao chamar uma nova senha.
* **Persistência:** Os contadores de senha e o histórico são salvos no `localStorage` do navegador, mantendo o estado entre sessões.
* **Rodapé Informativo:** Exibe informações de contato da ETEC (Instagram e Telefone/WhatsApp).
* **Layout Responsivo:** Interface adaptável a diferentes tamanhos de tela.

## 🚀 Como Usar

1.  **Executando a Aplicação:**
    * Como este é um projeto contido em um único arquivo HTML, basta baixar o arquivo (`senha.html).
    * Abra este arquivo HTML em qualquer navegador web moderno (Google Chrome, Firefox, Edge, etc.).

2.  **Operação (Atalhos de Teclado):**
    * **Tecla `N`**: Chama a próxima senha da fila normal.
    * **Tecla `P`**: Chama a próxima senha da fila prioritária.
    * **Tecla `Q`**: Reinicia todos os contadores de senha (normal e prioritária) para zero e limpa o histórico de chamadas. Uma mensagem "toast" confirmará a ação.

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estrutura da página.
* **Tailwind CSS:** Framework CSS para estilização rápida e responsiva.
* **JavaScript (Vanilla JS):** Lógica de funcionamento do sistema, manipulação do DOM e interações.
* **Tone.js:** Biblioteca JavaScript para geração de feedback sonoro.
* **Google Fonts (Inter, Orbitron):** Para a tipografia da aplicação.

## 📂 Estrutura do Projeto

O projeto consiste em um único arquivo HTML que embute todo o CSS (via Tailwind CDN e estilos inline) e JavaScript necessários para seu funcionamento.

* `senha.html`: Arquivo principal da aplicação.

## 🎬 Vídeo Institucional

O sistema possui um espaço reservado para um vídeo institucional. Para utilizá-lo:

1.  Localize a tag `<video id="videoInstitucional" ...>` no arquivo HTML.
2.  Altere o atributo `src` dentro da tag `<source>` para o caminho do seu arquivo de vídeo local ou URL.
    ```html
    <video id="videoInstitucional" ...>
        <source src="SEU_CAMINHO_PARA_O_VIDEO.mp4" type="video/mp4">
        Seu navegador não suporta o elemento de vídeo.
    </video>
    ```
    Substitua `SEU_CAMINHO_PARA_O_VIDEO.mp4` pelo nome e caminho corretos do seu arquivo de vídeo.

## 📞 Contato ETEC

As informações de contato da ETEC Adolpho Arruda Mello podem ser encontradas no rodapé da aplicação.

## 🔮 Possíveis Melhorias Futuras

* Integração com um backend para gerenciamento centralizado de senhas e estatísticas.
* Múltiplos guichês/pontos de chamada.
* Painel administrativo para configuração e visualização de relatórios.
* Customização de sons de chamada.
* Impressão de senhas (se aplicável ao fluxo).
