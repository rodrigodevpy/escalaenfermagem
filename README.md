# Escala Enfermagem

App web (PWA) para montar a escala de enfermagem e distribuir os quartos entre os técnicos. Funciona offline e pode ser instalado no celular ou computador. Os dados ficam salvos no próprio aparelho.

## Recursos

- **Equipe**: cadastro de enfermeiros e técnicos de enfermagem, cada um com cor e função.
- **Regras de escala**: plantão de 12h a cada N dias (padrão 12x36), X plantões seguidos antes de 1 folga, e mínimo de enfermeiros/técnicos por dia (dias abaixo do mínimo ganham ⚠️).
- **Alteração de escala**: por dia, marque plantão extra, folga ou ausência; ou faça uma troca de plantão entre dois membros. Para mudar o ciclo de forma permanente use "Ajustar início do mês".
- **Quartos**: cadastro individual ou em lote, com nível de complexidade (1 Baixa, 2 Média, 3 Alta).
- **Distribuição**: o botão "Planejar e distribuir" reparte os quartos entre os técnicos de plantão no dia escolhido, equilibrando a carga (soma dos níveis) e fazendo rodízio com os dias já planejados. Dá para mover quartos manualmente.
- **PDF por técnico**: um PDF com os quartos e a complexidade de cada um, ou um único PDF com uma página por técnico. É gerado no próprio app, sem internet.
- **Instalar como app**: banner e opção no menu (no iPhone: Compartilhar → Adicionar à Tela de Início).
- **Backup**: exportar e importar os dados em `.json`.

## Como usar

1. Cadastre a equipe em **＋ Membro** (informe o dia do 1º plantão).
2. Na aba **Quartos**, cadastre os quartos e o nível de cada um.
3. Na aba **Distribuição**, escolha o dia, toque em **Planejar e distribuir** e gere os PDFs.

## Publicação

Arquivos estáticos (`index.html`, `sw.js`, `manifest.json`): basta hospedar em qualquer servidor estático com HTTPS (por exemplo GitHub Pages).
