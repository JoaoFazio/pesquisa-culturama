# Formulário de Pesquisa - Culturama

Este projeto é um exercício prático e profundo de **validação de formulário moderna, semântica e acessível**. O foco principal não foi a estilização, mas sim a implementação de uma experiência de usuário (UX) robusta, que fornece feedback de validação *apenas após a interação do usuário*.

O projeto foi desenvolvido como parte da formação de HTML e CSS da Alura e evoluiu para um estudo de caso sobre o uso correto de pseudo-classes CSS e semântica de HTML5.

## 🚀 Link para o Deploy (GitHub Pages)

**Acesse e teste o formulário ao vivo aqui:**
[**https://JoaoFazio.github.io/nome-do-repositorio/**](https://JoaoFazio.github.io/pesquisa-culturama/)

## 📸 Demo da Validação Interativa

A imagem abaixo não mostra o formulário, mas sim a **lógica de validação em ação**. Note como os campos têm três estados diferentes (verde, vermelho e cinza) *baseado na interação do usuário*, provando que a validação não polui a tela ao carregar.

 <img width="733" height="936" alt="pesquisa-culturama" src="https://github.com/user-attachments/assets/7fd099cc-5388-4014-9445-a94f0e610163" />

* **Nome (Verde):** Está válido (`:user-valid`) após o preenchimento correto.
* **Idade (Vermelho):** Está inválido (`:user-invalid`) pois é `required` e o usuário interagiu, mas deixou em branco.
* **Email (Vermelho):** Está inválido (`:user-invalid`) pois o `type="email"` do HTML detectou um padrão incorreto.
* **Telefone (Cinza):** Está intocado. Prova que a validação só é aplicada após a interação.

## 🛠️ Habilidades e Conceitos Aplicados

Este projeto demonstra o domínio dos pilares de formulários web profissionais:

* **Validação CSS Moderna:** Uso das pseudo-classes `:user-valid` e `:user-invalid` para fornecer feedback de UX interativo. Isso evita a poluição visual de campos inválidos ao carregar a página, um problema comum com o `:invalid` tradicional.
* **Validação Semântica de HTML5:** O CSS funciona apenas porque o HTML está correto.
    * **Input Types Corretos:** Uso de `type="email"`, `type="date"`, `type="tel"`, `type="number"`, `type="file"`, e `type="color"`.
    * **Atributos de Validação:** Uso de `required`, `pattern` (para o telefone), `min`/`max` (para a idade).
* **Acessibilidade (a11y) e Semântica:**
    * **Labels Explícitas:** Uso correto do `<label for="id">` em absolutamente todos os campos de entrada, garantindo a usabilidade para leitores de tela.
    * **Agrupamento Lógico:** Uso de `<fieldset>` e `<legend>` para agrupar seções do formulário (Dados Pessoais, Perfil), melhorando a navegação.
    * **Instruções Claras:** Uso de `aria-describedby` para associar campos a textos de ajuda (como no campo de telefone).
* **Tipos de Entrada Avançados:**
    * Uso de `<select>` e `<option>` (com `value=""` e `required` para forçar a validação) para listas definidas.
    * Uso de `<datalist>` para sugestões de preenchimento (Estilo Musical).
    * Uso de `<textarea>` para campos de texto longo.
* **Fluxo de Múltiplas Páginas:** O formulário usa `method="get"` (para fins de demo) e redireciona para uma página de `sucesso.html` após o envio válido.

## 🏁 Como Executar Localmente

Este é um projeto estático, não necessita de instalação de dependências.

```bash
# 1. Clone o repositório
git clone [https://github.com/JoaoFazio/nome-do-repositorio.git](https://github.com/JoaoFazio/nome-do-repositorio.git)

# 2. Acesse a pasta
cd nome-do-repositorio

# 3. Abra o arquivo `index.html` no seu navegador
```
## 👨‍💻 Autor

Feito por João Gabriel (Não autoral).

* <a href="https://www.linkedin.com/in/jo%C3%A3o-gabriel-fazio-861186338/" target="_blank">LinkedIn</a>
* <a href="https://github.com/JoaoFazio" target="_blank">GitHub</a>
