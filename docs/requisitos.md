# Requisitos propostos para um cenário demonstrativo

## Requisitos funcionais
| Código | Funcionalidade | Prioridade | Critério de aceite proposto |
|---|---|---|---|
| RF01 | Autenticar usuários e aplicar perfis. | Alta | Usuário sem permissão não consegue aprovar. |
| RF02 | Registrar calibração e salvar rascunho. | Alta | Registros recebem identificadores diferentes e podem ser retomados. |
| RF03 | Importar medições de planilhas homologadas. | Alta | Importação preserva origem e não executa macros. |
| RF04 | Organizar características e repetições. | Alta | Medições iguais permanecem como repetições distintas. |
| RF05 | Validar campos, datas e unidades. | Alta | Pendência informa campo e motivo e bloqueia aprovação. |
| RF06 | Cadastrar instrumentos. | Alta | Código existente não cria instrumento duplicado. |
| RF07 | Vincular procedimento e revisão. | Alta | Revisão usada permanece no histórico. |
| RF08 | Vincular padrões de referência. | Alta | Padrão vencido na execução bloqueia o fluxo sem exceção autorizada. |
| RF09 | Complementar dados técnicos. | Alta | Campo obrigatório vazio gera pendência; zero não é ausência. |
| RF10 | Processar medições com regras aprovadas. | Alta | Fórmula sem aprovação não pode gerar resultado final. |
| RF11 | Calcular média e dispersão. | Alta | Caso de referência reproduz resultado aprovado. |
| RF12 | Calcular incerteza. | Alta | Componente obrigatório ausente impede conclusão. |
| RF13 | Avaliar tolerâncias. | Alta | Casos dentro, fora e no limite seguem a regra validada. |
| RF14 | Gerar prévia e PDF final. | Alta | PDF final só fica disponível após aprovação. |
| RF15 | Revisar, aprovar ou devolver. | Alta | Alteração posterior exige nova revisão e preserva versão aprovada. |
| RF16 | Consultar histórico. | Média | Busca por instrumento ou período recupera documentos autorizados. |

## Requisitos não funcionais
| Código | Qualidade | Prioridade | Como verificar |
|---|---|---|---|
| RNF01 | Segurança | Alta | Tentar acessar e aprovar sem permissão; conferir bloqueio no servidor. |
| RNF02 | Integridade | Alta | Interromper uma gravação; verificar que não ficam dados parciais. |
| RNF03 | Rastreabilidade | Alta | A partir do PDF, localizar origem, versão e responsável. |
| RNF04 | Usabilidade | Alta | Observar usuários representativos executando o fluxo básico. |
| RNF05 | Desempenho | Média | Definir volume e tempo-alvo com usuários antes de medir. |
| RNF06 | Recuperação | Alta | Restaurar cópia de teste e conferir registros e documentos. |
| RNF07 | Manutenção | Média | Alterar regra sem modificar certificados já aprovados. |
| RNF08 | Disponibilidade | Média | Definir janela de operação e medir interrupções. |
| RNF09 | Compatibilidade | Alta | Repetir importação nos navegadores e modelos homologados. |
| RNF10 | Conformidade | Alta | Validar regras e modelo com responsáveis técnicos; não presumir certificação. |

Nenhum desses critérios é apresentado como teste já executado. Prazos, metas numéricas e regras de cálculo exigem validação antes da implementação.
