# JF Central

Ferramentas de uso interno da Jaqueline Ferreira Assessoria Contábil: simuladores, calculadoras, checklists e modelos de documentos.
Cada simulador é um arquivo único (`index.html`), sem servidor e sem enviar dados para fora.

| Pasta | Simulador |
|---|---|
| `fator-r/` | Calculadora de Fator R (Simples Nacional) |
| `jornadas-remuneracao/` | Jornadas e Remuneração (v12, 23/11/2026) |
| `simples-hibrido/` | Simples Integral × Híbrido (CBS/IBS pelo regime regular) |
| `carta-reforma-tributaria/` | Carta de Adequação à Reforma Tributária |
| `calculadora-honorarios/` | Calculadora de Honorários (MEI, Simples, Presumido) |
| `proposta-revisao-2027/` | Proposta de Revisão para 2027 (Simples e Lucro Presumido), no papel timbrado |
| `minha-hora-financas/` | Minha Hora e Finanças: custo da hora, despesas do escritório (PJ) e pessoais (PF) |
| `contrato-proposta/` | Contrato e Proposta de Prestação de Serviços |
| `declaracoes-dp/` | Gerador de Declarações DP (cancelamento de término de experiência, orientação de demissão sem justa causa, termo de ciência e responsabilidade de não retirada de pró-labore) |
| `checklist-fechamento-mensal/` | Checklist de Fechamento Mensal |
| `checklist-obrigacoes-acessorias/` | Checklist de Obrigações Acessórias |
| `checklist-documentos-societarios/` | Checklist de Documentos Societários |
| `reforma-sem-surto/` | Reforma Sem Surto — para entender: resumo em linguagem simples do material de Reforma Tributária, com datas e fontes conferidas |
| `dominio/` | JF Domínio: guia dos 210 mapas do Sistema Domínio por departamento (as imagens ficam só no computador da Jaqueline; não entram no repositório) |

`index.html` na raiz é o menu: um seletor "O que você quer usar" que abre a ferramenta escolhida.

## Novo simulador
1. Criar a pasta `nome-do-simulador/` com um `index.html`.
2. Acrescentar uma `<option>` no seletor de `index.html` (raiz).

Apoio à conferência. Não substitui a análise da contadora nem a legislação vigente.

**Buscar CNPJ (opcional):** Fator R, Contrato e Proposta, Declarações DP, Proposta de Revisão 2027, Jornadas e os dois checklists (Fechamento e Obrigações) têm o botão "Buscar CNPJ". Só envia o CNPJ ao BrasilAPI (terceiros, espelho da base da Receita) depois de confirmação na tela. Não grava nada. Dados podem estar defasados: conferir no Comprovante da Receita.

O botão também lista o CNAE principal e os secundários e, na Calculadora de Fator R, marca a elegibilidade quando algum CNAE consta na lista curta da LC 123, art. 18 (principal: "Sujeita ao Fator R"; só secundário: "Atividade mista"). A lista de CNAEs está no código de cada ferramenta (objeto `DB`) e deve ser ampliada e conferida na Resolução CGSN 140/2018.

**Salvamento automático (F5 zera):** Fator R, Contrato e Proposta, Declarações DP, Proposta de Revisão 2027, Jornadas, os dois checklists (Fechamento e Obrigações), Carta de Adequação e Simples × Híbrido guardam o que é digitado neste navegador (nada é enviado). O botão "Limpar" apaga, com confirmação em dois cliques. Atenção: o dado fica neste computador; limpe antes de usar em máquina de outra pessoa.

**CNPJs já consultados:** depois de cada Buscar CNPJ, a ferramenta guarda no navegador o CNPJ, o nome e o resultado. Ao digitar o CNPJ (ou escolher na lista que aparece), os campos e o resultado voltam sem nova consulta. O botão "Apagar CNPJs salvos" limpa a lista, com confirmação em dois cliques. O F5 não apaga essa lista.
