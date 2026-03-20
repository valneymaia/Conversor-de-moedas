# App de Conversão de Moedas (React Native + Expo)

Aplicativo mobile de conversão de moedas feito em **React Native** usando **Expo**.

## Funcionalidades
- Converter valores entre moedas (ex.: BRL, USD, EUR)
- Escolher moeda de origem e moeda de destino
- Inserir valor manualmente e ver o resultado instantaneamente
- Atualizar cotação (online) *(se aplicável no seu app)*

## Tecnologias
- React Native
- Expo (Expo Dev Client / Expo Go)
- JavaScript/TypeScript *(ajuste conforme seu projeto)*
- API de câmbio *(ajuste conforme seu projeto — ex.: ExchangeRate API, Frankfurter, etc.)*

## Requisitos
- Node.js (recomendado: versão LTS)
- npm / yarn / pnpm
- Expo CLI (via `npx`)
- Um dispositivo com **Expo Go** instalado **ou** emulador Android/iOS

## Como rodar o projeto

### 1) Instalar dependências
```bash
npm install
# ou
yarn
# ou
pnpm install
```

### 2) Iniciar o Expo
```bash
npx expo start
```

### 3) Abrir no celular
- Abra o app **Expo Go**
- Escaneie o QR Code exibido no terminal/navegador

## Variáveis de ambiente (se usar API)
Se o app usa alguma API com chave, crie um arquivo `.env` (ou o formato que você estiver usando) e adicione:

```env
EXPO_PUBLIC_EXCHANGE_API_KEY=coloque_sua_chave_aqui
EXPO_PUBLIC_EXCHANGE_API_URL=https://...
```

> Ajuste os nomes acima para os que seu projeto realmente utiliza.

## Estrutura (exemplo)
> Ajuste para refletir a estrutura real do seu projeto.

- `src/`
  - `components/`
  - `screens/`
  - `services/` (requisições para API)
  - `utils/`
- `App.tsx` / `App.js`

## Como gerar build (opcional)
Se você usa **EAS Build**:

```bash
npm install -g eas-cli
eas login
eas build:configure
eas build --platform android
# ou
eas build --platform ios
```

## Prints / Demonstração
Adicione aqui imagens do app ou um GIF:

- `./docs/screenshot-1.png`
- `./docs/screenshot-2.png`

## Próximas melhorias (ideias)
- Histórico de conversões
- Cache/offline das últimas cotações
- Gráfico de variação da moeda
- Suporte a mais moedas e favoritos

## Licença
Defina a licença do seu projeto (MIT, Apache-2.0, etc.) ou remova esta seção.
