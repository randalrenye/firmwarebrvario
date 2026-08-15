# Histórico de versões

Todas as mudanças relevantes do firmware BRVARIO Normal serão documentadas
neste arquivo a partir da versão 3.6.

## 3.8 - 2026-08-14

### VARIO DINÂMICO

- Adicionado controle `DYNAMIC_ON` e `DYNAMIC_OFF` pelo aplicativo BRVARIO.
- Configuração gravada na memória e restaurada automaticamente ao ligar.
- `DYNAMIC_ON` mantido como padrão de fábrica e após restaurar as configurações.
- Primeiro pulso dinâmico ampliado para as configurações de ascendência de
  +0,10, +0,30 e +0,50 m/s, atuando até abaixo de +1,50 m/s.
- Em +1,50 m/s ou acima, o som utiliza imediatamente a curva normal.
- Com o recurso desligado, frequências, beeps e a cadência normal permanecem
  ativos, incluindo os ajustes introduzidos na versão 3.7.

### Compatibilidade

- Migração automática mantém o recurso ligado em aparelhos atualizados sem
  apagar as demais preferências existentes.
- Versão interna atualizada para 3.8.
- Mantido o nome `novobrvario.ino.bin` para compatibilidade com a atualização
  OTA do aplicativo BRVARIO.

## 3.7 - 2026-08-03

### Áudio

- Cadência de subida levemente mais lenta entre +0,10 m/s e +1,00 m/s.
- Curva de pausa inspirada no BRVARIO E-PAPER, aplicada de forma suave e
  preservando a frequência e a duração original dos beeps.
- Retorno progressivo à cadência já validada em +1,00 m/s, sem alterar o
  comportamento nas ascendências superiores.

### Compatibilidade

- Versão interna atualizada para 3.7.
- Mantido o nome `novobrvario.ino.bin` para compatibilidade com a atualização
  OTA do aplicativo BRVARIO.

## 3.6 - 2026-08-03

### VARIO DINÂMICO

- Transformado em uma indicação de entrada executada uma vez por nova subida.
- Partida aproximadamente 15% mais grave, seguida por recuperação progressiva
  da frequência em duas fases.
- Duração do pulso dinâmico ajustada entre 495 ms e 460 ms em cada faixa de
  0,10 m/s.
- Rearme somente após 2 segundos contínuos abaixo do limiar de saída, evitando
  repetição causada por oscilações rápidas do filtro.
- Modulação mantida até o final do pulso mesmo se o valor do vario atravessar a
  próxima faixa durante o beep.

### Áudio

- Frequências de subida e pré-termal reduzidas em 30 Hz para um timbre
  levemente mais grave.
- Curvas e cadências normais preservadas.
- Removidas lacunas de cálculo entre as faixas de subida, especialmente nas
  transições próximas de +2,0 m/s e +5,0 m/s.

### Compatibilidade

- Versão interna atualizada para 3.6.
- Mantido o nome `novobrvario.ino.bin` para compatibilidade com a atualização
  OTA do aplicativo BRVARIO.

## Versões anteriores

As notas e os binários das versões anteriores permanecem disponíveis na
[página de Releases](https://github.com/randalrenye/firmwarebrvario/releases).
