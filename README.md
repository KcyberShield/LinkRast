# LinkRast

Ferramenta de extração de links em páginas.

---

**Descrição**:  
Este script é um simples web crawler que percorre todas as páginas linkadas a partir de uma URL inicial fornecida. Ele coleta e exibe todos os links encontrados durante o rastreamento.

## Funcionalidades
- **Rastreia Páginas Web**: Começa a partir de uma URL inicial e rastreia todas as páginas linkadas.
- **Filtra Links Válidos**: Apenas URLs válidas (não âncoras) são consideradas durante o rastreamento.
- **Controle de Páginas Visitadas**: Evita visitar a mesma página mais de uma vez.


### Requisitos
- Python 3.x
- Bibliotecas: `requests`, `beautifulsoup4`, `argparse`

### Execução
1. Instale as bibliotecas necessárias:
   ```bash
   pip install requests beautifulsoup4
   ```

2. Execute o script passando a URL inicial como argumento:
   ```bash
   python LinkRast.py "https://exemplo.com"
   ```

3. O script exibirá todas as páginas encontradas durante o rastreamento.

## Exemplo de Uso
```bash
python LinkRast.py "https://exemplo.com"
```

## Observações
- O script captura exceções durante o acesso às páginas e continua o rastreamento mesmo que erros de rede ocorram.
- Os links são exibidos em ordem alfabética após o rastreamento ser concluído.

