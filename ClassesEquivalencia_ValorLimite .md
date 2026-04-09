# Atv – Particionamento em Classes de Equivalência e Análise do Valor Limite
Aluna: Tâmara Thais Lourenço de Carvalho | Matricula: 20232014040040

---

## Q1 – Função de Desconto

### Contexto
A função recebe duas entradas: **Cliente** (A, B ou C) e **Quantidade de itens (Qtd)**, variando de 1 a 1000.  
A saída é o **Desconto aplicado**, conforme regras específicas para cada cliente.

---

### Classes de Equivalência

- **Cliente**
  - Válido: A, B, C
  - Inválido: qualquer outro (ex.: D)

- **Quantidade**
  - Válida: 1 ≤ Qtd ≤ 1000
  - Inválida: Qtd < 1 ou Qtd > 1000

---

### Casos de Teste

#### Valores Limite
- Qtd = 1 → válido  
- Qtd = 1000 → válido  
- Qtd = 0 → inválido  
- Qtd = 1001 → inválido  

#### Exemplos Válidos
- Cliente A, Qtd = 7 → Saída: Sem desconto  
- Cliente A, Qtd = 50 → Saída: 5%  
- Cliente A, Qtd = 200 → Saída: 10%  
- Cliente B, Qtd = 5 → Saída: 5%  
- Cliente B, Qtd = 80 → Saída: 15%  
- Cliente B, Qtd = 300 → Saída: 25%  
- Cliente C, Qtd = 3 → Saída: Sem desconto  
- Cliente C, Qtd = 45 → Saída: 20%  
- Cliente C, Qtd = 500 → Saída: 25%  

#### Exemplos Inválidos
- Cliente D, Qtd = 20 → Cliente inválido  
- Cliente B, Qtd = 1500 → Quantidade inválida  
- Cliente C, Qtd = 0 → Quantidade inválida  

---

## Q2 – Inclusão de Contato na Agenda

### Contexto
A função de inclusão de contato recebe três entradas: **Nome**, **Telefone** e **Email**.  
As regras são:  
1. Todo contato deve ter telefone.  
2. Telefone deve ser único.  
3. Telefone deve ter entre 8 e 15 dígitos.  
4. Email deve seguir o formato alfanumérico *@*.*.  

---

### Classes de Equivalência

- **Nome**
  - Válido: preenchido
  - Inválido: nulo

- **Telefone**
  - Válido: único, 8–15 dígitos
  - Inválido: duplicado, <8 dígitos, >15 dígitos

- **Email**
  - Válido: formato correto *@*.* com letras e números
  - Inválido: fora do padrão

---

### Casos de Teste

#### Valores Limite
- Telefone com 8 dígitos → válido  
- Telefone com 15 dígitos → válido  
- Telefone com 7 dígitos → inválido  
- Telefone com 16 dígitos → inválido  

#### Exemplos Válidos
- Nome = Tâmara  
- Telefone = 987654322  
- Email = tamararuby@gmail.com  

#### Exemplos Inválidos
- Nome = Tâmara, Telefone = 987654321, Email = null → campo nulo  
- Nome = Tâmara, Telefone duplicado → inválido  
- Nome = Tâmara, Telefone = 2124567 → inválido (<8 dígitos)  
- Nome = Tâmara, Telefone = 1234567891000234 → inválido (>15 dígitos)  
- Nome = Tâmara, Email = tamararubygmailcom → inválido (não tem o @ e .)  

---

## Conclusão
Os casos de teste elaborados garantem q a cobertura de **classes válidas e inválidas**, além de **valores limite**, garantindo que a função de desconto e a inclusão de contatos sejam correatemte validadas.
