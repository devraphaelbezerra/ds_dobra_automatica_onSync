# 🔧 Correção Temporária da Dobra Automática no TOTVS RMS
    Dataset Customizado OnSync: ds_dobra_automatica_onSync.js

Este projeto apresenta uma solução temporária desenvolvida no Fluig para corrigir falhas no processo de **Dobra Automática** do TOTVS RMS. A rotina identifica notas fiscais que não foram devidamente processadas e gera as correspondentes em uma agenda alternativa por meio de uma API Visual Mix, garantindo a integridade e continuidade dos processos operacionais enquanto aguarda a solução oficial do problema.

---

## 🎯 Objetivo

- Detectar notas fiscais não processadas pela Dobra Automática.
- Gerar automaticamente as notas correspondentes em uma agenda alternativa via API.
- Assegurar a continuidade das operações enquanto aguarda a solução oficial do problema pela TOTVS.

---

## ⚙️ Funcionamento

1. A rotina é executada periodicamente no Fluig.
2. Realiza consultas no banco de dados para identificar notas fiscais não processadas.
3. Utiliza uma API para gerar as notas correspondentes em uma agenda alternativa.
4. Registra logs das operações realizadas para auditoria e acompanhamento.

---

## 🛠️ Tecnologias Utilizadas

- **TOTVS Fluig** (JavaScript)
- **APIs RESTful**
- **Banco de Dados** (Oracle/PostgreSQL)

---

## 📌 Observações

- Esta é uma solução temporária e deve ser descontinuada após a resolução oficial do problema pela TOTVS.
- Recomenda-se monitorar os logs regularmente para garantir o correto funcionamento da rotina.
- Certifique-se de que as notas geradas estejam sendo corretamente associadas aos documentos fiscais na agenda alternativa.

---

## 📝 Exemplo de Log (simulação)

```txt
[INFO] Iniciando verificação na tabela de notas fiscais
[INFO] Encontrados 5 registros de notas não processadas
[UPDATE] Registro ID 101 atualizado na agenda alternativa
[UPDATE] Registro ID 102 atualizado na agenda alternativa
[UPDATE] Registro ID 105 atualizado na agenda alternativa
[COMMIT] Alterações salvas com sucesso
[INFO] Execução finalizada em 1.5 segundos
