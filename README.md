# Repositório do Projeto · Concessão das Travessias do Estado de São Paulo (Acquavias)

Consolidado em **23/11/2026**. Reúne todo o contexto do projeto: memória, conversas (threads), artefatos publicados, arquivos usados e gerados, e os geradores (scripts) dos relatórios.

- **Contrato:** SPI nº 012/2026 (Acquavias × ARTESP), travessias litorâneas e do Vale do Paraíba/Billings.
- **Início da operação:** 09/11/2026 (ano contratual 1: 09/11/2026 a 08/11/2027).
- **Verificador Independente:** ECR Engenharia. **Sistema operacional:** DRIVE/SIGO (fornecedor Innovia).

## Estrutura desta pasta

| Pasta / arquivo | O que tem |
|---|---|
| `README.md` | Este índice, regras-chave e pendências |
| `01-memoria/` | Cópia da memória do projeto (`MEMORY.md` + 30 fichas por assunto) |
| `02-threads/` | Um resumo por thread (objetivo, achados, decisões, entregáveis) + `00-chat-do-projeto.md` |
| `03-artefatos/artefatos-publicados.md` | Os 6 artefatos do claude.ai com links |
| `04-inventario-arquivos.md` | Inventário de todos os 854 arquivos de `/mnt/project-files/` (caminho, tamanho, data) |
| `05-geradores-e-textos/` | Cópia dos scripts (.py, .sh, .js), consultas Power Query/DAX, JSONs e textos .md, nos mesmos caminhos de origem |

Os arquivos originais **continuam onde estavam**; nada foi movido. PDFs do contrato, planilhas grandes e relatórios gerados ficam indexados no inventário.

## Threads (em ordem cronológica)

| # | Data | Thread | Tipo |
|---|---|---|---|
| 00 | 26/10–19/11 | Chat do projeto (fórmulas Excel, API, e-mails) | Consulta |
| 01 | 26/10 | Verificar exigência de balança registrada no INMETRO | Contrato |
| 02 | 27/10 | Localizar serviços de vistoria na fase de transição | Contrato |
| 03 | 27/10 | Explicar cláusula de excludentes nos indicadores | Contrato |
| 04 | 27/10 | Explicação da metodologia REV08 ao verificador | Artefato |
| 05 | 28/10 | Conferir mínimo mensal de Cananéia/Ilha Comprida | Contrato |
| 06 | 28/10 | Verificar exigência de peso estimado por veículo | Contrato |
| 07 | 29/10 | Medir tempo de fila com OCR das cabines | Contrato |
| 08 | 28/10 | Justificar cláusula de embarcação substituta no afretamento | Texto |
| 09 | 27/10 e 11/11 | Fichas Obsidian dos indicadores e da contraprestação | .md |
| 10 | 03/11 | Encaminhar contrato BK para o administrativo | .md |
| 11 | 03–10/11 | PDFs de grade de horários por travessia | PDF + artefato |
| 12 | 04 e 11/11 | Definição de embarque e viagem | Contrato |
| 13 | 06–07/11 | Informativo dos indicadores de desempenho | PDF |
| 14 | 09/11 | Relatório de viagens Santos–Guarujá (Excel) | Excel |
| 15 | 09/11 | Programação de abastecimento | PDF/JPG |
| 16 | 09/11 | Campos exigidos para balança rodoviária | Contrato |
| 17 | 09/11 | Revisar indicadores de outubro + pontualidade Cananéia | Análise + artefato |
| 18 | 10–12/11 | Comparativo Santos–Guarujá 05h–10h e relatórios gerais | PDF |
| 19 | 10–19/11 | **Relatórios diários Diretoria e Operação** (thread principal: Power BI, financeiro, operação, ocorrências, template, fila × navios) | PDF/Excel/BI |
| 20 | 10–19/11 | Projetar receita das viagens + volume SSI e volume médio | PDF/Excel |
| 21 | 11/11 | Peso na amostragem do IAU | Contrato |
| 22 | 11/11 | Indicadores de SS/Ilhabela por serviço | Contrato |
| 23 | 12/11 | Informativo de classificação de expurgos | PDF |
| 24 | 13/11 | IAD zerado de outubro + dados à ARTESP + SIGO | Análise + artefatos |
| 25 | 17/11 | Horário escolar das 05h45 em Cananéia | Contrato |
| 26 | 18/11 | Tempo de escoamento e intervalo de atendimento da demanda | PDF |
| 27 | 19/11 | Quantitativo de viagens do Vale do Paraíba | Revisão |

## Regras e decisões que valem para o projeto todo

**Identidade visual Acquavias:** fonte Lato; #005B7F (azul), #00B5AD (turquesa), #003A52 (azul escuro), apoio #B7DCE6, #5BC8C2, #00968F. Sem vermelho/rosa no financeiro. Logo no cabeçalho, rodapé "Acquavias · Análise de Performance", A4.

**Relatórios:** não citar fontes externas nem nomes de arquivo (BD_QT, BSM, REV, Anexo); "Quantitativo"/"Projeção". Operação sem citar indicadores nem expurgo, salvo pedido. Cada revisão entregue com **nome de arquivo novo** "(v. dd-mm hhhmm)".

**Receita (Diretoria):** viagens ÷ 4 × R$ 2.314,05 × 0,75 (FO ano 1) = **R$ 433,88 por viagem (A)**; (B) a 60% = **R$ 260,33**. (A) = até a projeção FIX/DEM do dia; (B) = acima disso. Atraso não exclui da receita. Multiplicador por perna (cada saída = 1 viagem). ÷4 vem de QV = 4 × PMF (Anexo 14, Tabela 1). R$ 2.314,05 não consta do contrato (vem da proposta).

**Orçamento de novembro/2026:** 34.084 viagens (09–30/11) → **R$ 14.788.515**.

**Operação:** tolerância de horário fixo −2/+5 min; viagem com atraso > 15 min = não realizada (IVP). Expurgo só para indicadores: horário dentro da janela de ocorrência dos **incisos i–v** do Anexo 8 item 2.6 (tipo conferido pelo comentário; vi depende da ARTESP) e viagem não feita/atrasada. Expurgos valem para IVP, IHP, ITP e IAD.

**Grades:** horários fixos um a um; conforme demanda em faixas cheias "a cada até X min"; "00h00" e nunca "24h00"; Tabela 5 (Bertioga) exige só intervalo por sentido, não saída simultânea; falta de tripulação não é justificativa (Anexo 3A 2.5.13); alteração de grade = 30 dias de aviso (2.5.8/2.5.9); programação excepcional só conta com ≥ 65% de ocupação (2.6.9).

**Indicadores:** HOC = 16 h × 2 sentidos × dias (992 h em outubro); espera 0 = hora boa; SS–Ilhabela apurada como uma travessia, exceto IAD (veículos × passageiros); IAU sem peso por nº de pesquisas, só ICHC × 2.

**Dados à ARTESP:** acesso em tempo real (Anexo 3A 2.11.10.3); contrato não fala em "exportação"; fornecer quando solicitado em 10 dias úteis (Cl. 24.1 xvi). Ao Verificador: extrações semanais toda segunda enquanto a API não existir (proposta de 19/11).

## Pendências em aberto (última situação conhecida)

1. Madrugada de Natividade, Paraitinga e Varginha: defasagem entre pontas de **30 min (REV08) ou ~10 min (praticado)**; hoje gera falso atraso no relatório da Operação.
2. Cananéia–Continente: confirmar de qual margem é a saída das 04:00.
3. Santos–Vicente de Carvalho sábado: lacuna de saídas de Santos 16h–22h (confirmar se era até 22h40).
4. Bertioga: 40 min sem saída de Bertioga 16h00–16h40 (entra 10 min na janela de 20 min).
5. Natividade: Pouso Alto e Bairro Alto em coluna única; confirmar se devem ter horários separados.
6. Quantitativo Vale do Paraíba: aplicar correções (total 84.463, fatores documentados, feriados, abas desatualizadas).
7. REV08: 66 células de set/2027 sem recálculo; grafia "Taquecetuba"; viagens fracionadas em João Basso e Bororé.
8. PMF mensal ou anual (Anexo 14, Tabela 1) e origem do PUP R$ 2.314,05.
9. Critério de consolidação de IAD/ITP/IRE em SS–Ilhabela e de IAU entre travessias, a formalizar com VI/ARTESP.
10. Horário escolar 05h45 em Cananéia: ofício à ARTESP + resposta à ouvidoria (oferecido redigir).
11. Responsáveis por indicador (proposta do informativo) a validar.
12. API DRIVE/SIGO → Verificador: em solicitação ao fornecedor desde 19/11/2026.

## Onde está cada gerador (principais)

| Relatório | Gerador mais recente |
|---|---|
| Grades de horários (PDF) | `grades-horarios-rev09/gerador/gen.py` |
| Relatório diário Diretoria/Operação | `relatorios-viagens/relatorio-diario/gerador/gerar.sh` (ver `LEIAME.txt`) |
| Financeiro mensal (1 página) | `relatorios-viagens/relatorio-financeiro/gerador/projecao/gen_1pag18.py` |
| Operação (diário e acumulado) | `relatorios-viagens/relatorio-financeiro/gerador/operacao/gen_op21.py` |
| Receita do ano 1 | `relatorios-viagens/relatorio-financeiro/gerador/gerar.py` |
| Relatório geral todas as travessias | `relatorios-viagens/gerador-geral/build.py` |
| Comparativo SG 05–10h | `relatorios-viagens/comparativo-sg-0911-1611/gerador/gen.py` (e `gen_du.py`) |
| Fila × passagens de navio | `relatorios-viagens/relatorio-fila-navios/gerador/gen_exec.py` |
| Tempo de escoamento / intervalo | `relatorios-viagens/tempo-escoamento/gerador/gen.py`, `gen_int.py` |
| Registro de ocorrências | `relatorios-viagens/registro-ocorrencias/gerador/gen_reg.py`, `classif.py` |
| Volume SSI do dia | `relatorios-viagens/volume-ssi/gerador/gen.py` |
| Volume médio por hora/barco | `relatorios-viagens/volume-medio/gerador/gen7.py` |
| Projeção feriado 20/11 | `relatorios-viagens/projecao-2011/gerador/gen.py` |
| Template de horários | `template-horarios/gerador/corrigir.py`, `duas_abas.py`, `aba_correcoes.py` |
| Bases do Power BI | `power-bi-travessias/gerador-bases/build_bases.py` |
| Programação de abastecimento | `programacao-abastecimento/gerador/gen.py` |

Cópias desses scripts estão em `05-geradores-e-textos/`, nos mesmos caminhos. Os PDFs são renderizados com `print.js` (Chromium/Playwright).
