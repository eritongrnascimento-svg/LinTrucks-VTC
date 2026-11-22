# LinTrucks VTC 0.1.0-26 — Windows e Linux

Atualização restrita aos áudios e seus gatilhos, usando as três gravações fornecidas pelo titular, sem clonagem de voz:

- **Carga coletada:** Frase 1, uma vez por viagem; o controle fica salvo para não repetir ao reiniciar.
- **Combustível abaixo de 50% da capacidade do tanque:** Frase 2, uma vez enquanto permanecer abaixo desse nível. Rearma após abastecer até pelo menos 50%.
- **Entrada no excesso acima da tolerância:** bipe curto, sem sirene nem voz; substitui o aviso antigo com fala.
- **Ocorrência interna registrada após mais de 10 segundos contínuos:** sirene curta seguida da Frase 3. O áudio só é solicitado depois de a gravação local confirmar uma nova ocorrência; reenvios não repetem a fala.
- Multas recebidas do próprio jogo continuam com registro imediato e também usam o aviso da Frase 3 após a confirmação local.
- Reprodução sem sobreposição; avisos de velocidade e multa têm prioridade sobre as falas comuns. O botão de teste existente reproduz o bipe.

**Preservados:** tolerâncias, duração de mais de 10 segundos, classes Arcade/Realista/Platina, valores e processamento das multas, autenticação, HUD e sincronização. O controle de som continua sem interferir no registro. Nenhuma alteração na VPS.

Feche jogo e cliente antes de instalar. Baixe o Setup para Windows ou AppImage/.deb para Linux e confira `SHA256SUMS.txt`. Linux continua exigindo glibc 2.35+ e dependências do sistema. Os fontes proprietários permanecem privados; os avisos/fontes de terceiros continuam disponíveis à parte.

## Compatibilidade com Fedora 45

O patch Linux mantém a versão 0.1.0-26 e acrescenta o RPM nativo x86_64 para Fedora 45. O AppImage e o DEB atualizados incluem a documentação e os metadados do aplicativo. O cliente permanece proprietário.
