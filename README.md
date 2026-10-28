# Site Dra. Lara Beatriz | Odontologia e Saúde

Site de uma página (one-page) da clínica **Dra. Lara Beatriz Odontologia e Saúde**, em Jacobina do Piauí - PI. Feito em HTML, CSS e um pouco de JavaScript puro, sem frameworks e sem etapa de instalação.

**Versão:** atual (28/10/2026)

---

## Arquivos

| Arquivo | Para que serve |
|---|---|
| `index.html` | O site inteiro. Já traz a foto e as logos embutidas, então funciona sozinho. |
| `foto-dra-lara.jpg` | Foto da doutora usada na seção "Sobre" (635 × 819 px, resolução original). |
| `logo-branca.png` | Logo branca com fundo transparente, ampliada a partir da arte do Instagram. |
| `logo.jpg` | Logo redonda original, ampliada. Usada como ícone da aba do navegador. |

As imagens soltas são cópias de reserva. Para usar o site, basta o `index.html`.

---

## Seções do site

1. **Topo:** logo, telefone clicável e botão "Agendar consulta". Fica transparente e escurece ao rolar.
2. **Início:** título, botões de ação e logo em destaque.
3. **Sobre a doutora:** foto da Dra. Lara e apresentação.
4. **Tratamentos:** consulta, limpeza, clareamento, alinhadores, restaurações e canal.
5. **Alinhadores:** lista de benefícios, aproveitada do cartaz da clínica.
6. **Como funciona:** passo a passo do atendimento.
7. **Localização:** mapa, endereço, telefone e botões "Ver no Google Maps" e "Como chegar".
8. **Dúvidas frequentes.**
9. **Chamada final** com WhatsApp e telefone, mais o rodapé.
10. **Botão flutuante de WhatsApp** em todas as páginas.

---

## Como editar

### Telefone e WhatsApp

Número atual: **(86) 99427-4867** (+55 86 99427-4867).

Para trocar, procure no `index.html` a linha:

```js
const NUM="5586994274867";
```

Use `55` + DDD + número, só dígitos. Ao trocar essa linha, o script atualiza os links de ligação e de WhatsApp. Os números que aparecem escritos na tela (topo, localização, chamada final e rodapé) também são reescritos pelo script no formato `(DD) XXXXX-XXXX`.

Se quiser mudar o número no texto estático também, procure por `(86) 99427-4867` e por `5586994274867`.

### Cores

As cores da marca ficam no começo do arquivo, no bloco `:root`:

| Variável | Cor | Uso |
|---|---|---|
| `--wine` | `#984050` | Vinho da marca (botões, destaques) |
| `--char` | `#2B2B2D` | Grafite escuro (fundos) |
| `--blush` | `#F2E6E6` | Rosa-claro (fundo da logo) |
| `--rose` | `#C98F88` | Dourado rosado (detalhes) |
| `--salmon` | `#F4B6A8` | Rosa-salmão (destaques em fundo escuro) |

Trocar um valor ali muda o site inteiro.

### Textos

Todos os textos estão direto no HTML. Procure pelo título da seção, por exemplo "Tratamentos" ou "Dúvidas frequentes", e edite.

### Foto e logo

As imagens estão embutidas no `index.html` em formato base64. Para trocar a foto, substitua o conteúdo do `src` da imagem dentro de `<div class="portrait">`. Mantenha a proporção da foto, já que o código trava a proporção 635:819 para ela nunca ficar esticada.

---

## Mapa e localização

- O botão **"Ver no Google Maps"** abre o perfil **Dra.Lara Beatriz Odontologia** no Google Maps.
- O botão **"Como chegar"** abre a rota até as coordenadas `-7.9309067, -41.1961512`.
- O mapa dentro da página usa o identificador do perfil (`cid=4012377720498669988`).
- O Plus Code da clínica é `3R93+JG`.

O mapa embutido precisa de internet e pode não aparecer em prévias que bloqueiam o Google. Abra o arquivo no Chrome ou publique o site para ver o mapa.

---

## Como publicar

O site é um arquivo estático. Qualquer hospedagem serve:

- Enviar o `index.html` para a hospedagem (Netlify, GitHub Pages, Vercel, Hostinger etc.) como página inicial.
- Opcional: registrar um domínio próprio e apontá-lo para a hospedagem.

Fontes (Playfair Display e Manrope) são carregadas do Google Fonts. Se estiver sem internet, o site usa fontes de reserva do sistema.

---

## Pendências e pontos para conferir

- **Horário de atendimento:** hoje aparece "consulte pelo WhatsApp". Falta o horário real.
- **Tratamentos e perguntas frequentes:** os textos são sugestões genéricas. Confirmar com a clínica o que ela realmente oferece, inclusive atendimento infantil e formas de pagamento.
- **Endereço completo:** o Google Maps mostra só "Jacobina do Piauí - PI". Se houver rua e número, incluir.
- **Logo:** a logo original tinha só 150 px. A versão branca foi ampliada a partir da arte do Instagram. Se existir o arquivo original em alta resolução ou vetorial (SVG/PDF), substituir para ficar ainda mais nítida.
- **Redes sociais:** ainda não há link para o Instagram da clínica.
- **Teste em aparelhos:** conferir o site no celular e em computador, principalmente o botão de WhatsApp, a ligação e o mapa.

---

## Créditos de conteúdo

- Foto e logo: material fornecido pela clínica.
- Benefícios dos alinhadores: baseados no cartaz da clínica.
- Dados de localização: perfil da clínica no Google Maps.
