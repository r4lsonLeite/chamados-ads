# chamados-ads

API de chamados de suporte desenvolvida com Flask.

## Estudante

**Nome completo:** jose Railson Leite da silva

## Objetivo do projeto

Criar a estrutura inicial de uma API de chamados de suporte com Flask, usando o `uv` para gerenciar o ambiente e as dependências. Nesta etapa (semana 01), a API possui apenas a rota inicial `GET /`, que confirma que o serviço está em funcionamento. Cadastro de chamados e banco de dados serão implementados nas próximas etapas.

## Requisitos

- [uv](https://docs.astral.sh/uv/) instalado
- Python 3.14 (o `uv` baixa automaticamente, se necessário)

## Instalação das dependências

Na raiz do repositório, execute:

```bash
uv sync --locked
```

Esse comando cria o ambiente virtual `.venv` e instala exatamente as versões registradas no `uv.lock`.

## Execução da aplicação

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

A aplicação ficará disponível em `http://localhost:5000`. No GitHub Codespaces, abra a porta 5000 pela aba **Portas/Ports**.

## Acessando a rota inicial

Com a aplicação em execução, acesse `http://localhost:5000/` no navegador ou use o terminal:

```bash
curl -i http://localhost:5000/
```

Resposta esperada:

- Status: `200 OK`
- Cabeçalho: `Content-Type: application/json`
- Corpo:

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```
