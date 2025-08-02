# ✅ Atividade Prática – Testes com Jqwik: Validação de CPF

---

## 🎯 Objetivo

Esta atividade prática tem como finalidade aplicar testes **baseados em propriedades** usando a biblioteca **Jqwik**, com foco na **validação de CPF**. A proposta é simular cenários realistas, explorar contraprovas e aprimorar a lógica implementada com base nas descobertas dos testes.

---

## 🗂️ Estrutura do Projeto

validador-cpf-jqwik/

├── src/

│ ├── main/java/cpf/

│ │ ├── ValidadorCPF.java # Classe com a lógica de validação

│ │ └── CPF.java # Classe auxiliar para geração de CPF válido

│ └── test/java/cpf/

│ └── ValidadorCPFPropertyTest.java # Classe com os testes baseados em propriedades

├── pom.xml # Configuração do projeto Maven com Jqwik e AssertJ

├── README.md # Este arquivo

└── .github/workflows/test.yml # Pipeline de testes automáticos com GitHub Actions

---

## 📜 Regras e Instruções

### Parte 1 – Execução Inicial

1. Faça o clone do projeto:
   
   git clone https://github.com/SEU_USUARIO/validador-cpf-jqwik.git
   cd validador-cpf-jqwik

2. Execute os testes para verificar o comportamento atual:
  
   mvn clean test

3. Observe os resultados e, se possível, contraprovas geradas pelo Jqwik.
   
### Parte 2 – Modificação Intencional

1. Modifique o método calcularDigito da classe ValidadorCPF.java (ex.: altere o peso usado no cálculo).

2. Execute os testes novamente e observe se o Jqwik detecta os erros (contraprovas).

3. Adicione uma nova propriedade de teste:

"CPFs válidos com um dígito trocado devem ser rejeitados".

### Parte 3 - Entrega

Entregar:

- Código alterado (em um fork ou PR)
- Screenshot de uma contraprova (se houver)
- Um pequeno relatório respondendo:
  - O que foi detectado?
  - Como os testes baseados em propriedades ajudaram?
  - Isso seria fácil de encontrar com testes unitários tradicionais?

## 🛠️ Ferramentas Utilizadas

- Jqwik – Testes baseados em propriedades
- AssertJ – Verificações expressivas nos testes
- GitHub Actions – Integração contínua e automação de testes

## 📊 Critérios de Avaliação

| Critério                                 | Peso                          |
|------------------------------------------|-------------------------------|
| Execução correta dos testes              | 2,0                           |
| Alteração intencional e contraprovas     | 2,5                           |
| Clareza e coerência da nova propriedade  | 2,0                           |
| Análise e reflexão no relatório          | 3,5                           |
| **Total**                                | **10,0**                      |  
  
