# Hellshit Loader

⚠️ **Aviso**: Este projeto é destinado exclusivamente a fins educacionais, de pesquisa e análise de técnicas de carregamento de executáveis. O uso indevido é de total responsabilidade do usuário.

---

## 💀 Sobre o Projeto

**Hellshit Loader** é um projeto desenvolvido com foco em técnicas avançadas de carregamento e injeção de executáveis no Windows. Ele explora métodos como:

- Mapeamento manual de executáveis (manual mapping)
- Syscalls diretas e indiretas
- Relocations em tempo de execução
- Evitação de IOC comuns (Indicators of Compromise)
- Técnicas anti-debug e anti-emulação

O objetivo é criar um loader funcional para fins de **estudo em segurança ofensiva**, **engenharia reversa** e **entendimento de internals do Windows**.

---

## 🧠 Funcionalidades

- [x] Carregamento manual de PE em processo suspenso
- [x] Suporte a relocations
- [x] Resolução de imports manualmente (opcional)
- [x] Uso de syscalls diretas para evasão
- [x] Compatível com executáveis 64 bits

---

## 🛠️ Tecnologias e Ferramentas

- Linguagem: **C / C++**
- Plataforma: **Windows (x64)**
- Toolchain: `mingw-w64`, `MSVC`, `NASM` (se aplicável)
- Bibliotecas: Nenhuma externa (somente WinAPI / NTDLL)

---

## 🚀 Como Usar

1. Compile o projeto:
    ```bash
    gcc -o hellshit_loader.exe main.c -masm=intel -lntdll -Wall
    ```

2. Execute:
    ```bash
    .\hellshit_loader.exe
    ```

3. Certifique-se de que o executável a ser carregado está no mesmo diretório ou forneça o caminho completo.

⚠️ **Nota**: É altamente recomendado executar em ambiente de testes / sandbox.

---

## 🧪 Testado em

- Windows 10 x64 (Builds 1809 a 22H2)
- Windows 11 (em VMs)
- Compatível com processos .exe legítimos e stub loaders

---

## 📚 Referências

- [Windows Internals - Pavel Yosifovich et al.]
- [Syscall Research by Sektor7, MDSec, and others]
- [PE File Format - Microsoft Docs]
- [Process Hollowing & Manual Mapping - MalwareTech, ired.team]

---

## ⚠️ Aviso Legal

> Este projeto foi criado com fins exclusivamente educacionais e de pesquisa. O autor não se responsabiliza por qualquer uso indevido ou malicioso deste código. Use sempre em conformidade com a legislação do seu país e com princípios éticos.

---

## 📄 Licença

MIT License. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## ✉️ Contato

Para dúvidas, sugestões ou contribuições:
**[seu email ou github aqui]**

