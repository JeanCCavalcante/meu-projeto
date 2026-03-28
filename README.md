# POO - Simulador - Nível 06 

![](https://assets.dio.me/a3lDo6zumV5NBm0M52pLFacavELX19r716XGQbaYR50/f:webp/q:80/L2FydGljbGVzL2NvdmVyL2NkNzQzODBiLTQwNjMtNDU2OC1iODVlLWYyZDBkMDZmYTJkMS5qcGc)

### 1. Criando um Repositório

Existem duas formas principais de começar um projeto com Git: criando um do zero ou copiando um que já existe na internet (como no GitHub ou GitLab).

* **Para criar um repositório do zero na sua máquina:**
    Abra o terminal na pasta do seu projeto e digite:
    ```bash
    git init
    ```
    *Isso inicializa o Git na pasta atual, permitindo que ele comece a rastrear os arquivos.*

* **Para copiar (clonar) um repositório existente:**
    ```bash
    git clone <url-do-repositorio>
    ```
    *Exemplo: `git clone https://github.com/usuario/projeto.git`. Isso baixa o projeto inteiro para a sua máquina.*

---

### 2. Subindo suas Alterações (O ciclo básico)

Depois de modificar ou criar arquivos, você precisa "salvar" e enviar essas mudanças para o repositório remoto. Esse processo tem três passos principais:

1.  **Verificar o que mudou (opcional, mas recomendado):**
    ```bash
    git status
    ```
    *Mostra quais arquivos foram modificados, adicionados ou deletados.*

2.  **Adicionar as mudanças à "área de preparação" (Staging):**
    ```bash
    git add .
    ```
    *O ponto `.` adiciona **todos** os arquivos modificados. Se quiser adicionar apenas um arquivo específico, use `git add nome-do-arquivo.txt`.*

3.  **Salvar as mudanças com uma mensagem (Commit):**
    ```bash
    git commit -m "Sua mensagem explicando o que foi feito"
    ```
    *Exemplo: `git commit -m "Adiciona a página de login"`.*

4.  **Enviar para o repositório online (Push):**
    ```bash
    git push origin <nome-da-sua-branch>
    ```
    *Se você estiver na branch principal (geralmente chamada de `main` ou `master`), o comando será `git push origin main`.*

---

### 3. Criando e Navegando em Branches

As *branches* (ramificações) servem para você criar novas funcionalidades sem mexer no código principal do projeto.

* **Para ver todas as branches existentes no seu computador:**
    ```bash
    git branch
    ```

* **Para criar uma branch nova e já mudar para ela:**
    ```bash
    git checkout -b <nome-da-nova-branch>
    ```
    *Exemplo: `git checkout -b funcionalidade-carrinho`.*

* **Para mudar para uma branch que já existe:**
    ```bash
    git checkout <nome-da-branch>
    ```

---

### 4. Atualizando sua Branch

Se outras pessoas estiverem trabalhando no mesmo projeto (ou se você fez alterações direto no GitHub), você precisa baixar essas atualizações para o seu computador.

* **Para puxar as atualizações do repositório remoto para a sua branch atual:**
    ```bash
    git pull origin <nome-da-branch>
    ```
    *Exemplo: Se você quer atualizar a sua branch com as novidades da branch principal, você vai até a sua branch e digita `git pull origin main`.*

---

### Resumo Rápido (Cheat Sheet)

| Ação | Comando |
| :--- | :--- |
| Iniciar repositório | `git init` |
| Clonar projeto | `git clone <url>` |
| Ver alterações | `git status` |
| Adicionar tudo | `git add .` |
| Salvar (Commit) | `git commit -m "mensagem"` |
| Enviar (Push) | `git push origin <branch>` |
| Criar e ir para branch | `git checkout -b <nome>` |
| Puxar atualizações | `git pull origin <branch>` |
