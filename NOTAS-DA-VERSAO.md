# Entrega Linux 0.1.0-25 e correção pontual Windows 0.1.0-24

- Linux: inicialização X11/XWayland, uma tentativa de fallback Mesa por software e erro de saída quando a interface não abre.
- Nova base de compilação: glibc 2.35+, para ampliar o alcance em relação ao pacote anterior (glibc 2.39+).
- AppImage utiliza bibliotecas do sistema. `--instalar-dependencias` usa o gerenciador da distribuição; `.deb` declara dependências para instalação pelo APT.
- AppImage inclui metadados de atualização e arquivo `.zsync` para ferramentas compatíveis com AppImageUpdate. O cliente não faz atualização automática internamente.
- Linux e Windows: perfil pode ser alterado respeitando os requisitos; a viagem mantém sua classe mesmo após multas, penalidades ou reinício do cliente. A correção Windows restringe-se à regra de classe e à orientação na tela de perfil.
- O instalador Windows mantém o nome e a versão 0.1.0-24 solicitados, com recompilação corretiva em 15/11/2026. Compare o SHA256 para distinguir do instalador original de 13/11.

**Instalação:** feche jogo e cliente anterior. No Linux, consulte `LEIA-ME-Linux.txt`. Dependências e repositórios precisam estar disponíveis; glibc anterior a 2.35 e Alpine/musl não são suportados. O HUD exige X11/XWayland.

**Validação:** testes automatizados e inicialização gráfica em ambiente isolado. Uma viagem real no ETS2/ATS e a compatibilidade com cada combinação de distribuição, driver e compositor precisam ser confirmadas em Linux nativo.

**Licenças:** os fontes do VTC são privados. Avisos e fontes de componentes de terceiros são fornecidos separadamente e permanecem sob suas próprias licenças.
