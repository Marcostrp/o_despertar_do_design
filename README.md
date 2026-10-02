<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://ai.google.dev/static/site-assets/images/share-ais-513315318.png" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/4b781074-afcb-489f-8cb8-76450bf1b3fc

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

---

## Visual Pixel Art (atualização)

O tabuleiro e os personagens agora são **pixel art gerada em código** (sem depender das imagens de IA):

- `src/utils/pixelTiles.ts` — pisos por bioma, paredes de tijolo, pilares, portais animados, baús e props.
- `src/utils/pixelCharacters.ts` — herói (idle, andar, dash, golpe, magia, dano), NPCs, monstros e cenário de batalha.
- `src/components/IsometricCanvas.tsx` — tabuleiro com ordenação de profundidade, tochas e iluminação.
- `src/components/TurnBasedBattle.tsx` — batalha usando os novos sprites animados.

Para mudar cores ou desenhos, edite as paletas no começo de cada função nesses arquivos.
