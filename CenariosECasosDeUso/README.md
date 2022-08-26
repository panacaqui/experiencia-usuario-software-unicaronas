# Caso de uso

![Caso de uso](CasoDeUso.jpeg)

# Cenários

## Cenário #01

### **Usuário realiza cadastro com e-mail acadêmico válido**

DADO QUE o usuário deseja se cadastrar no sistema<br>
QUANDO ele inserir o \<email> e \<senha><br>
E confirmar o \<codigo><br>
ENTÃO o cadastro será realizado, o usuário será redirecionado para a página de configurar agenda e exibirá uma \<mensagem><br>

### **Exemplo**
email: gustavo.ribeiro@discente.ufg.br<br>
senha: 12345678<br>
codigo: 123456<br>
mensagem: Cadastro realizado com sucesso<br>

---
## Cenário #02

### **Usuário realiza cadastro com e-mail não acadêmico**

DADO QUE o usuário deseja se cadastrar no sistema<br>
QUANDO ele inserir o \<email> e \<senha><br>
ENTÃO o cadastro não será realizado e aparecerá uma \<mensagem><br>

### **Exemplo**
email: mail.gustavo.oliveira@gmail.com<br>
senha: 12345678<br>
mensagem: Cadastro não realizado, informe um e-mail acadêmico<br>

---
## Cenário #03

### **Usuário realiza cadastro com e-mail acadêmico inválido**

DADO QUE o usuário deseja se cadastrar no sistema<br>
QUANDO ele inserir o \<email> e \<senha><br>
E informar o \<código> de confirmação<br>
ENTÃO o cadastro não será realizado e aparecerá uma \<mensagem><br>

### **Exemplo**
email: mail.gustavo.oliveira@gmail.com<br>
senha: 12345678<br>
codigo: 2<br>
mensagem: Cadastro não realizado, código de confirmação inválido<br>

---
## Cenário #04

### **Usuário realiza login com dados inexistentes no sistema**

DADO QUE o usuário deseja realizar login no sistema<br>
QUANDO ele informar \<email> e \<senha><br>
ENTÃO o sistema não realizará o login e exibirá uma \<mensagem><br>

### **Exemplo**
email: gustavo.ribeiro@discente.ufg.br<br>
senha: 12345678<br>
mensagem: Usuário não encontrado<br>

---
## Cenário #05

### **Usuário realiza login com dados válidos**

DADO QUE o usuário deseja realizar login no sistema<br>
QUANDO ele informar \<email> e \<senha><br>
ENTÃO o sistema será redirecionado para a página de eventos<br>

### **Exemplo**
email: gustavo.ribeiro@discente.ufg.br<br>
senha: 12345678<br>

---
## Cenário #06

### **Passageiro busca por caronas**

DADO QUE um passageiro deseja buscar uma carona<br>
QUANDO ele informar o \<endereço de partida> e \<horario de partida> e o \<destino> e \<horario de chegada><br>
E confirmar a rota que aparecerá<br>
ENTÃO o sistema irá listar as caronas disponíveis para a rota e no horário desejado<br>

### **Exemplo**
endereço de partida: Rua Elvado Lodi, nº 100<br>
horario de partida: 10:00<br>
destino: Restaurante Universitário Samambaia<br>
horario de chegada: 12:00<br>

---
## Cenário #07

### **Passageiro seleciona uma carona**

DADO QUE o passageiro realizou uma busca por caronas<br>
QUANDO ele selecionar um dos resultado<br>
ENTÃO o sistema irá exibir os detalhes daquel carona<br>

---
## Cenário #08

### **Passageiro envia a solicitação de carona**

DADO QUE o passageiro visualizou os detalhes de uma carona<br>
QUANDO ele clicar em "solicitar carona"<br>
ENTÃO o sistema irá enviar uma notificação para o caronista e exibirá uma \<mensagem><br>

### **Exemplo**
mensagem: Solicitação de carona enviada com sucesso<br>

---
## Cenário #09

### **Usuário configura um dia da agenda**

DADO QUE um usuário esteja na página da agenda e deseja configurar um dia<br>
QUANDO ele informar o \<endereço de partida> e \<horario de partida> e o \<destino> e \<horario de chegada><br>
E confirmar a rota que aparecerá<br>
ENTÃO o sistema irá salvar a configuração para ser usada automaticamente em outras situações e exibirá uma \<mensagem><br>

### **Exemplo**
endereço de partida: Rua Elvado Lodi, nº 100<br>
horario de partida: 10:00<br>
destino: Restaurante Universitário Samambaia<br>
horario de chegada: 12:00<br>
mensagem: Configuração salva com sucesso<br>
