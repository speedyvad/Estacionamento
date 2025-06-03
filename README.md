# 🚗 Sistema de Estacionamento - WebApp Interativo

Este é um sistema de gerenciamento de estacionamento desenvolvido com **HTML, CSS e JavaScript puro**. Ele simula a entrada e saída de veículos em um estacionamento de 25 vagas, com uma interface moderna e responsiva, além de aplicar **regras de região geográfica** com base nas placas brasileiras.

## 📌 Funcionalidades

- ✅ Estacionamento visual com 25 vagas em grid 5x5
- 🕒 Cálculo de tempo e valor de permanência com tolerância de 15 minutos
- 💰 Tarifação adicional para veículos de fora das regiões Sudeste e Centro-Oeste
- 🧾 Geração de ticket com informações detalhadas
- 🌎 Reconhecimento de estado e região com base nos 3 primeiros caracteres da placa
- 🔎 Sistema visual de cores para distinguir vagas livres, ocupadas e com taxa extra
- ⚠️ Validação de formato de placas (padrão Mercosul: `LLLNLNN` como `ABC1D23`)
- 📱 Totalmente responsivo (mobile/tablet/desktop)

## 🧠 Tecnologias Utilizadas

- HTML5
- CSS3 (com gradientes, animações e media queries)
- JavaScript (DOM, validações, manipulação de datas)

## 📚 Regras de Negócio

- Apenas veículos das **regiões Sudeste e Centro-Oeste** podem estacionar sem taxa adicional.
- Veículos de outras regiões ainda podem estacionar, **mediante uma taxa extra de R$ 10,00**.
- O valor base do estacionamento é:
  - **R$ 10,00 até 3h**
  - **+ R$ 5,00 por hora adicional**
- Tolerância de até **15 minutos grátis** (sem cobrança)

## 🖼️ Interface

### 🅿️ Grid de Vagas
- Vagas livres: Verde
- Vagas ocupadas: Vermelho
- Vagas com taxa extra: Laranja com ícone 💰

### 🎫 Tickets
- Mostram placa, estado, região, tempo e valores
- Identificam a origem da placa com ícones:
  - 🌆 Sudeste
  - 🌾 Centro-Oeste
  - 🚫 Outras regiões

### ⚠️ Pop-up de Restrição
Quando um veículo de fora da área permitida tenta estacionar, um pop-up oferece a **opção de pagar a taxa extra** ou cancelar a entrada.

## 🚀 Como usar

1. Baixe ou clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/sistema-estacionamento.git
   ```
2. Abra o arquivo `index.html` no navegador.
3. Teste inserindo placas (ex: `ABC1D23`, `JKR2A45`, `HZZ4B32` etc.).

## 🔍 Exemplos de Placas Válidas

- **Sudeste:** `HAA1B23`, `KMA2C34`, `BFA3D45`
- **Centro-Oeste:** `JKA4E56`, `JWL5F67`, `NFB6G78`
- **Outras (taxa extra):** `JWA7H89` (Ceará), `NEA8I90` (Pará)

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

Feito com ❤️ para fins educacionais e de aprendizado.