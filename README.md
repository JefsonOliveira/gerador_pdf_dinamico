# Gerador de PDF Dinâmico

🚀 **Gerador de PDF Dinâmico** é um projeto desenvolvido como parte do curso #HoraDeCodar. Este projeto utiliza a biblioteca pdfmake para criar PDFs dinâmicos de forma eficiente e flexível.

## Funcionalidades

- 📄 **Criação de PDFs Dinâmicos**: Gera PDFs com conteúdo dinâmico conforme a necessidade do usuário.
- 🖼️ **Suporte a Imagens**: Insira imagens nos seus PDFs.
- 🎨 **Estilização Customizável**: Personalize o estilo do PDF, incluindo fontes, cores e layout.

## Tecnologias Utilizadas

- **Biblioteca de Geração de PDF**: pdfmake
- **Frontend**: ReactJS (se aplicável)
- **Estilo**: CSS (se aplicável)

## Instalação e Uso

Para rodar o projeto localmente, siga os passos abaixo:

1. Clone o repositório (somente leitura):

```sh
git clone https://github.com/JefsonOliveira/gerador_pdf_dinamico.git
```

2. Navegue até o diretório do projeto:
   ```sh
   cd gerador_pdf_dinamico
   ```
3. Instale as dependências:
   ```sh
   npm install
   ```
4. Inicie o servidor de desenvolvimento com Vite:
   ```sh
   npm run dev
   ```

O aplicativo estará disponível em `http://localhost:3000`.

## Exemplo de Uso

Aqui está um exemplo básico de como usar a biblioteca pdfmake no projeto:

```javascript
import pdfMake from "pdfmake/build/pdfmake";
import pdfFonts from "pdfmake/build/vfs_fonts";

pdfMake.vfs = pdfFonts.pdfMake.vfs;

const docDefinition = {
  content: [
    { text: "Este é um exemplo de PDF!", style: "header" },
    "Texto normal",
    { text: "Outro texto com estilo", style: "anotherStyle" },
    { text: "Texto embutido", style: "header" },
  ],
  styles: {
    header: {
      fontSize: 22,
      bold: true,
    },
    anotherStyle: {
      fontSize: 16,
      italics: true,
    },
  },
};

pdfMake.createPdf(docDefinition).download();
```

## Contato

Para dúvidas ou mais informações, entre em contato:

- **Nome**: Jefson K Oliveira
- **Email**: kaironoliveira16@gmail.com
- **LinkedIn**: [Meu Perfil](https://www.linkedin.com/in/jefson-oliveira-a92a62206/)
