# BePop API

- RF (Requisito funcional)
- RNF (Requisito não funcional)
- RN (Regra de negócio)

---
## Login

**RF**

- [] Deve ser possível criar uma conta utilizando login social (Facebook e Google), além de email/senha.
- [] Deve ser possível realizar o login social
- [] Deve ser possível realizar o logout

**RNF**

- [] Utilizar o Firebase Auth para login

**RN**

- [] Não deve ser possível criar uma conta com e-mail já existente

---
## Concurso

**RF**

- [] Deve ser possível cadastrar um concurso
- [] Deve ser possível listar um concurso
- [] Deve ser possível atualizar um concurso
- [] Deve ser possível excluir um concurso
- [] Deve ser possível se inscrever em um concurso
- [] Deve ser possível realizar o upload do comprovante de pagamento da inscrição de um concurso
- [] Deve ser possível curtir/descurtir o vídeo de um concurso
- [] Deve ser possível compartilhar um concurso
- [] Deve ser possível disparar uma notificação push de confirmação de pagamento

**RNF**

- [] Utilizar o Firestore/ElephantSQL para armazenar os dados de concursos
- [] Utilizar o CloudStorage para armazenar os comprovantes de pagamento
- [] Utilizar o Firebase Cloud Messaging(FCM) para envio de pushs
- [] Utilizar o mongoDB/FireStore para armazenar o device token do FCM

**RN**

- [] Não deve ser possível se inscrever mais de uma vez no mesmo concurso
- [] Não deve ser possível atualizar os dados de um concurso caso seja criado por outro membro
- [] Não deve ser possível excluir um concurso caso já exista participantes inscritos
- [] Não deve ser possível excluir um concurso não existente
- [] Não deve ser possível se desinscrever de um concurso
- [] Não deve ser possível curtir mais uma vez o mesmo vídeo de um concurso

---
## Perfil

**RF**

- [] Deve ser possível atualizar os dados cadastrais
- [] Deve ser possível atualizar os dados bancários
- [] Deve ser possível listar dos dados de atividade
- [] Deve ser possível deletar sua conta

**RN**

- [] Não deve ser possível apagar os dados cadastrais
- [] Não deve ser possível apagar os dados bancários

---
## Admin

**RF**

- [] Deve ser possível encerrar um concurso
- [] Deve ser possível listar os comprovantes de pagamentos pendentes
- [] Deve ser possível confirmar a inscrição de um membro em um concurso (via comprovante)
