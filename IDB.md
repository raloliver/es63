# INDEXEDDB

- Com o IDB não abrimos uma conexão, mas sim, solicitamos uma requisição de abertura
- Precisamos lidar com um tríade de eventos disparados quando tentamos acessar um banco no IndexedDB.
    - openRequest.onupgradeneeded: cria ou altera um banco já existente.
    - openRequest.onsucess: realizado sempre que a conexão é bem sucedida.
    - openRequest.onerror: chamado quando existe algum erro na conexão.