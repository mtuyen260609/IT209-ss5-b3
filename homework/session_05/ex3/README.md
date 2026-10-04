# BÃ¡o cÃ¡o BÃ i 3: Xá»­ lÃ½ xung Ä‘á»™t phá»©c táº¡p trong quÃ¡ trÃ¬nh Rebase

## Chi tiáº¿t cÃ¡c láº§n phÃ¡t sinh conflict
1. **Láº§n 1 (Táº¡i commit `feat: change port`):**
   - **MÃ´ táº£:** Xung Ä‘á»™t táº¡i file `config.json` do nhÃ¡nh main sá»­a port thÃ nh 8081 vÃ  thÃªm env, trong khi nhÃ¡nh feature sá»­a port thÃ nh 9000.
   - **CÃ¡ch giáº£i quyáº¿t:** Má»Ÿ file `config.json`, xÃ³a bá» cÃ¡c dáº¥u hiá»‡u xung Ä‘á»™t (`<<<<<<<`, `=======`, `>>>>>>>`). Giá»¯ láº¡i port lÃ  9000 (cá»§a feature) vÃ  giá»¯ láº¡i env (cá»§a main).
   - Cháº¡y `git add config.json` vÃ  `git rebase --continue`.

2. **Láº§n 2 (Táº¡i commit `feat: enable debug`):**
   - **MÃ´ táº£:** Xung Ä‘á»™t táº¡i file `config.json` á»Ÿ dÃ²ng `debug`.
   - **CÃ¡ch giáº£i quyáº¿t:** Má»Ÿ file, cáº­p nháº­t `debug` thÃ nh `true`.
   - Cháº¡y `git add config.json` vÃ  `git rebase --continue`.

## Lá»‹ch sá»­ sau khi hoÃ n thÃ nh
```
* 462e5cf feat: enable debug
* fcb3c36 feat: change port
* 630183b add env config
* a9c7c18 update port on main
* 3734a56 init config
```
