# Experiment

Пошаговое инструкция повторении эксперимента на `Ubuntu (64-bit)`:
### PreRequirements
1. Скачать `nuxmv`:
   - Скачиваем из `https://nuxmv.fbk.eu/`
   - `tar xf nuXmv-2.1.0-linux64.tar.xz`
   - Добавляем путь в переменную `$PATH`
2. Скачать `BIP toolset`
   - Скачиваем из `https://www-verimag.imag.fr/-BIP-Tools-93-?lang=en`
   - `tar xf bip-full-2015.04-RC7_x86_64.xz`
   - Добавляем путь в переменную `$PATH`
3. Проверяем на маленьком тесте `one smart contract`
   - Для автоматизации теста я написал маленький соурс `run_nuxmv.tcl`, который поможет запустить `nuxmv` быстрее
   - `$NUXMV_EXE -source run_nuxmv.tcl > out.out`
   - Внутри логов ищем `specification`
  **Мой результат:**
<img width="1126" height="104" alt="image" src="https://github.com/user-attachments/assets/c23f7804-9e05-49bc-8542-5814a203a6f7" />
  **Результат Автора**
<img width="942" height="127" alt="image" src="https://github.com/user-attachments/assets/2f7afbce-7df1-4a4d-ba4c-a8d8578e848f" />
     
