# Heartforge

Modpack do nosso servidor (Minecraft 1.21.1, NeoForge 21.1.265). Este repositório guarda o pack no formato de
atualização automática: o seu ATLauncher confere este repositório sempre que você abre o jogo e baixa só o que mudou.

## Instalar (uma vez só)

1. Importe o **Heartforge-Jogadores.zip** no ATLauncher (Add Instance → Import). Ele já traz o atualizador
   (`packwiz-installer-bootstrap.jar`).
2. Na instância do Heartforge, abra as configurações da instância e vá na aba **Commands**.
3. Marque **Enable commands** e cole no campo **Pre-Launch Command**:

   ```
   $INST_JAVA -jar packwiz-installer-bootstrap.jar -s client https://raw.githubusercontent.com/0ArS0/heartforge/main/pack.toml
   ```

4. Salve e jogue. A cada abertura aparece uma janelinha conferindo o pack; quando houver novidade, ela baixa e o
   jogo abre já atualizado.

O servidor: `sp20.razehost.com.br:25604`

## Para quem mantém o pack

Gerado a partir da instância por `heartforge-pack-tools/gen_packwiz.py`. Mods que estão no Modrinth são baixados
direto de lá (aqui só fica o link e o hash); o resto fica guardado neste repositório. Arquivos pessoais (opções,
vídeo, controles) são instalados uma vez e nunca sobrescritos.
