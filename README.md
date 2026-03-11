# Documentação da Aplicação

## Objetivo da Aplicação

A aplicação tem como objetivo permitir o **cadastro e gerenciamento de cursos** em um sistema. Através dela, o usuário pode inserir informações de novos cursos, validar os dados informados, verificar se o cadastro foi realizado corretamente e também excluir cursos cadastrados.

O sistema busca garantir que os dados sejam inseridos corretamente, evitando campos vazios, dados inválidos e respeitando limites de caracteres definidos para cada campo.

---

# Principais Fluxos Disponíveis

## 1. Cadastro de Curso

Permite ao usuário inserir as informações necessárias para cadastrar um novo curso no sistema.

Etapas principais do fluxo:

1. Acessar a tela de cadastro de curso  
2. Preencher os campos do formulário  
3. Validar os campos obrigatórios  
4. Validar o tipo de dados inseridos (números e letras)  
5. Validar a quantidade de caracteres permitidos  
6. Enviar o formulário para realizar o cadastro  

---

## 2. Validação de Dados

Durante o processo de cadastro, o sistema realiza validações para garantir a integridade das informações inseridas.

Principais validações:

- Verificação de **campos em branco**
- Validação de **campos que aceitam apenas números**
- Validação de **campos que aceitam apenas letras**
- Validação da **quantidade mínima ou máxima de caracteres**

Essas validações evitam inconsistências e garantem a qualidade dos dados cadastrados.

---

## 3. Persistência do Cadastro

Após o cadastro de um curso, o sistema deve manter as informações armazenadas corretamente.

Fluxo validado:

1. Realizar o cadastro de um curso
2. Sair do sistema
3. Entrar novamente no sistema
4. Verificar se o curso continua cadastrado

Esse fluxo garante que os dados foram realmente persistidos no sistema.

---

## 4. Consulta do Curso Cadastrado

Permite verificar se o curso foi salvo corretamente após o cadastro.

Esse fluxo garante que:

- O curso aparece na listagem
- As informações cadastradas estão corretas

---

## 5. Exclusão de Curso

Permite remover um curso previamente cadastrado.

Fluxo:

1. Localizar o curso cadastrado
2. Executar a ação de exclusão
3. Confirmar que o curso foi removido da listagem

---

# Pontos Críticos do Sistema para Testes

Algumas funcionalidades do sistema possuem maior impacto no funcionamento da aplicação.
Site não esta funcional para ser repassado ao usuário.


A funcionalidade de exclusão deve garantir que:

- O curso seja removido corretamente
- A listagem seja atualizada
- O curso não possa mais ser encontrado após a exclusão
