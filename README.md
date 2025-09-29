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
   - Внутри логов ищем `specification` (`cat out.out | grep specification`)

**Мой результат:**
<img width="1126" height="104" alt="image" src="https://github.com/user-attachments/assets/c23f7804-9e05-49bc-8542-5814a203a6f7" />

**Результат Автора:**
<img width="942" height="127" alt="image" src="https://github.com/user-attachments/assets/2f7afbce-7df1-4a4d-ba4c-a8d8578e848f" />
     
**Вывод:** Результаты совподают

### Остальные Мини-тесты:

### DAO

**Мой результат:**
<img width="1781" height="105" alt="image" src="https://github.com/user-attachments/assets/dd716e8e-2180-4966-8816-54a155a86c8e" />


**Результат Автора:**
<img width="1660" height="215" alt="image" src="https://github.com/user-attachments/assets/8589d138-f170-414d-bd33-dcd10ac99cdf" />

### Global

**Мой результат:**
<img width="1787" height="154" alt="image" src="https://github.com/user-attachments/assets/85e46c04-38e0-49e1-8b64-148c831f1927" />


**Результат Автора:**
<img width="1660" height="317" alt="image" src="https://github.com/user-attachments/assets/d95dbfd6-7cdd-41b8-aa5f-7295add0adec" />

### Gold game

**Мой результат:**
<img width="1787" height="101" alt="image" src="https://github.com/user-attachments/assets/5d9540a8-8964-47a5-b4c6-05883e41275f" />


**Результат Автора:**
<img width="1787" height="192" alt="image" src="https://github.com/user-attachments/assets/9035fdaa-2ac5-45da-aa7c-155b573f60cf" />

**Вывод:** Во всех мини-тестах результаты совподают

### Большой эксперимент

- внутри файла run_nuxmv.tcl меняем<br>
`"A-Verification-Approach-for-Composite-Smart-Contracts-Security-using-FSM/one smart contract/addsub/addsub.smv" -> "A-Verification-Approach-for-Composite-Smart-Contracts-Security-using-FSM/composite smart contract/Travel_Agency_system_example.smv"
- `$NUXMV_EXE -source run_nuxmv.tcl > out.out`
- Ждем примерно 38 часов((
- Внутри логов ищем `specification`

**Мой результат:**
<img width="1743" height="207" alt="image" src="https://github.com/user-attachments/assets/0d56d4b8-a6b7-49a1-bcb9-05633a5955f7" />


**Результат Автора:**
<img width="3051" height="1502" alt="image" src="https://github.com/user-attachments/assets/b779df28-77ef-45bf-a864-70430f63ce0b" />
     
**Вывод:** Результаты совподают

- Результаты мини-тестов взяты напрямую из (github) [https://github.com/mouhamad-almakhour/A-Verification-Approach-for-Composite-Smart-Contracts-Security-using-FSM/blob/8a531248eedd65d0fad71f6d82a7f02d0c158eab/one%20smart%20contract/addsub/Verification_result]
- Результат эксперимента из (статьи) [https://www.sciencedirect.com/science/article/pii/S1319157822003111]
