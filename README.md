# Chai & Pages

HCI Lab 07: Figma-to-website conversion.
A responsive one-page site for a small bookshop and café in Gulberg, Lahore.

- Figma design: https://www.figma.com/design/8X3PFzPAdX0SSAYFHDjKQU/HCI-Lab-07
- Live site: https://shaigansaeed.github.io/Chai-and-Pages/
- 
## Stack
Semantic HTML5 + Tailwind CSS (CDN, no build step). Design tokens in `index.html` (`tailwind.config`) match the Figma `Tokens` variables.

## Figma MCP
`.vscode/mcp.json` connects VS Code to the remote Figma MCP server (`https://mcp.figma.com/mcp`).

## Assets
`assets/` holds SVGs exported from the Figma file: `hero.svg` plus the icon set.

## Run locally
Open the folder in VS Code and use the Live Server extension on `index.html`, or run `npx serve`.

## Responsive checks
Tested at 1440 px (3-column grid), 768 px (2 columns) and 375 px (1 column, menu button). No `position: absolute` is used for layout.

## Accessibility
Landmarks (`header`, `nav`, `main`, `section`, `footer`), skip link, visible focus and hover states, every input has a bound `<label>`, descriptive `alt` text on images, `aria-label` on the decorative book covers.

## Deploy
Vercel: `npx vercel --prod` from this folder (static site, no build command).
