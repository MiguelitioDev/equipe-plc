# Objetivos de Desenvolvimento — Carlos

**Foco:** Inimigos, Movimentação de Ameaças e Sistema de Colisão  
**Arquivos de Atuação:** `src/missao/Inimigo.java` (Criar) e `src/missao/Missao.java` (Modificar)

---

## 🎯 Objetivos Principais

### 1. Criar a Classe `Inimigo.java`
* **O que fazer:** Modelar a entidade de inimigo com coordenadas `(x, y)`.
* **Regras:**
  * Atributos privados com métodos getters e setters/movimentação.
  * Deve permitir consultar e alterar sua posição no mapa.

### 2. Implementar a Movimentação dos Inimigos em `Missao.java`
* **O que fazer:** Criar o controle da lista de inimigos e a rotina para movê-los a cada turno.
* **Regras:**
  * Adicionar uma lista (`List<Inimigo>`) dentro da classe `Missao`.
  * Criar método para adicionar inimigos e obter a lista de inimigos.
  * Criar método de movimentação que desloque cada inimigo no mapa após a ação do jogador.
  * **Obrigatório:** O movimento dos inimigos não pode ultrapassar as bordas do mapa (limites mínimos e máximos de X e Y).

### 3. Atualizar o Sistema de Colisão e Dano
* **O que fazer:** Expandir a checagem de colisão da missão para incluir os inimigos.
* **Regras:**
  * Verificar colisão tanto com `Asteroide` quanto com `Inimigo`.
  * Se a nave colidir (mesmo `X` e `Y`), aplicar perda de vida da nave (`nave.perderVida()`).
  * Tratar o encerramento do jogo quando a vida da nave zerar.

---

## 📋 Checklist de Entrega (Definition of Done)

- [x] Arquivo `Inimigo.java` criado e encapsulado no pacote `missao`.
- [x] Classe `Missao.java` gerenciando a coleção de inimigos.
- [x] Inimigos se movem a cada turno sem sair dos limites do mapa.
- [x] Colisão com inimigos detectada e vidas da nave decrementadas corretamente.
- [x] Jogo finaliza por derrota quando a vida da nave chega a 0.
- [x] Código compilando limpo com `javac -d out src/missao/*.java`.