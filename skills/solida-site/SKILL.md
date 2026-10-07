---
name: solida-site
version: 0.1.0
description: Desenvolve e valida o site institucional cinematográfico da Sólida usando uma adaptação do workflow Think/Act/Prove do Fable Method.
---

# Skill: Sólida Site

## Missão

Construir uma experiência institucional premium para a Sólida, com identidade visual oficial, cenas conectadas por scroll, WebGL/Three.js quando justificável, GSAP/ScrollTrigger, liquid glass e suporte a português, inglês e espanhol.

A experiência visual deve reforçar proteção, solidez, confiança e criatividade. Ela não pode prejudicar leitura, acessibilidade, desempenho ou conversão.

## Ordem de leitura

Leia antes de modificar:

1. `AGENTS.md`.
2. `skills/solida-site/references/project-context.md`.
3. `skills/solida-site/references/workflow.md`.
4. `skills/solida-site/references/acceptance-criteria.md`.
5. O `informacoes-do-projeto.md` e os materiais oficiais disponíveis na pasta do projeto.

## Workflow Think / Act / Prove

### Think

Antes de codificar, registre:

- objetivo da tarefa;
- estado atual do projeto;
- arquivos a ler e modificar;
- hipótese técnica;
- dependências e riscos;
- comportamento esperado em desktop, mobile, teclado e movimento reduzido;
- teste que provará a conclusão.

Se faltar uma informação essencial, marque como bloqueio ou escolha a alternativa reversível mais simples. Não invente.

### Act

- Faça uma alteração pequena e isolada.
- Preserve APIs, materiais e referências existentes.
- Prefira componentes e funções testáveis.
- Mantenha conteúdo, traduções e configuração fora da lógica de animação.
- Use um controlador central de progresso para as cenas.
- Evite múltiplos renderers e timelines concorrentes sem justificativa.

### Prove

Depois da alteração:

- execute lint, testes e build disponíveis;
- abra a aplicação localmente quando houver navegador;
- examine console e rede;
- valide dimensões desktop e mobile;
- capture screenshots ou vídeos dos estados importantes;
- compare o resultado com o critério de aceite;
- registre limitações e próxima tarefa.

Nunca escreva apenas “funciona”. Informe comando, resultado e evidência.

## Direção técnica

- Use Vite + TypeScript ou preserve a stack existente quando ela já estiver adequada.
- Use Three.js para a cena 3D e GSAP/ScrollTrigger para coreografia quando aprovados.
- Use o SVG oficial para o símbolo animado.
- Implemente lago e montanhas com custo controlado; água em shader é preferível a simulação física pesada.
- Carregue assets grandes progressivamente.
- Considere GLB/glTF, Draco, Meshopt e KTX2 apenas após medir o benefício.
- Faça o conteúdo essencial existir como HTML acessível.

## Cenas previstas

1. **Lago:** água, montanhas, pôr do sol, slogan e entrada.
2. **Travessia:** deslocamento de câmera entre montanhas e transição inspirada na referência autorizada.
3. **Símbolo:** símbolo oficial da Sólida se abre para permitir a passagem.
4. **Carrossel:** scroll vertical convertido em sequência horizontal com elemento central transformável.
5. **Contato:** chamada final, canais oficiais e retorno opcional ao início.

A referência Igloo e a referência MANA orientam comportamento e ritmo, mas não autorizam copiar marca, textos ou assets sem permissão registrada. O liquid glass do projeto da Sólida deve ser estudado e integrado sem substituir sua implementação por um efeito genérico.

## Idiomas

Suporte obrigatório a `pt-BR`, `en` e `es`.

- Preserve o sentido original.
- Não traduza conteúdo jurídico automaticamente sem revisão.
- Verifique que textos longos não quebram o layout.
- Use HTML para textos importantes, nunca somente texto desenhado no canvas.

## Desempenho

- Medir FPS e tempo de carregamento em aparelhos definidos.
- Reduzir resolução e pós-processamento em dispositivos limitados.
- Pausar animação quando a aba estiver oculta.
- Respeitar `prefers-reduced-motion`.
- Oferecer fallback sem WebGL.
- Não manter cenas invisíveis renderizando sem necessidade.

## Regras jurídicas e editoriais

A Sólida atua em direitos autorais, propriedade intelectual e registro de marcas. A interface pode ser informativa e administrativa, mas não deve prometer resultado, inventar prazo, criar depoimento ou substituir orientação jurídica profissional.

## Formato de relatório

Ao terminar, responda com:

```text
Tarefa:
Think:
Arquivos alterados:
Act:
Comandos executados:
Prove:
Limitações:
Próxima tarefa:
```
