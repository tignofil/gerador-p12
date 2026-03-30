# 🔐 Gerador de Certificado P12

Ferramenta web para geração de certificados **PKCS#12 (.p12)** autoassinados, desenvolvida para uso interno da equipe. Ideal para assinar documentos e PDFs.

> **100% client-side** — nenhum dado é enviado a servidores externos. Todo o processamento ocorre no navegador do usuário.

---

## ✨ Funcionalidades

- Geração de par de chaves RSA (1024, 2048 ou 4096 bits)
- Certificado X.509 autoassinado com SHA-256
- Campos configuráveis: CN, Organização, País, Estado, E-mail
- Validade personalizável (padrão: 365 dias)
- Proteção por senha com indicador de força
- Download direto do arquivo `.p12` no navegador
- Sem dependências de servidor — funciona como página estática

---

## 🚀 Como usar

Acesse diretamente pelo GitHub Pages:

```
https://tignofil.github.io/gerador-p12
```

Ou baixe o arquivo `index.html` e abra localmente no navegador.

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML / CSS / JS puro | Interface e lógica |
| [node-forge](https://github.com/digitalbazaar/forge) | Criptografia RSA e geração PKCS#12 |
| Google Fonts (Syne + DM Mono) | Tipografia |

---

## 📦 Deploy no GitHub Pages

1. Faça o fork ou clone deste repositório
2. Vá em **Settings → Pages**
3. Em **Branch**, selecione `main` e pasta `/root`
4. Clique em **Save**
5. Acesse a URL gerada em alguns minutos

---

## ⚠️ Avisos importantes

- Os certificados gerados são **autoassinados** e não são reconhecidos por autoridades certificadoras públicas (CAs)
- São adequados para uso interno, testes e assinatura de documentos em ambientes controlados
- Para uso em produção ou com validade jurídica, utilize uma CA homologada (ex: ICP-Brasil)
- **Guarde a senha do `.p12` em local seguro** — não é possível recuperá-la

---

## 🔒 Segurança

- Nenhuma chave privada, senha ou dado pessoal trafega pela rede
- Todo o código é aberto e auditável neste repositório
- A biblioteca node-forge é carregada via CDN do [cdnjs.cloudflare.com](https://cdnjs.cloudflare.com)

---

## 📄 Licença

MIT — livre para uso, modificação e distribuição.
