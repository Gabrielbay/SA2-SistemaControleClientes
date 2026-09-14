# Sistema de Controle de Clientes — SA2 Atividade 1

Codificação Back-End (SENAI) — sistema de console em C# que aplica os conceitos
de Programação Orientada a Objetos (abstração, herança, polimorfismo e
encapsulamento) a partir do diagrama de classes proposto na atividade.

## Diagrama de classes

- `Clientes` (classe-pai): `nome`, `endereco`, `valor`, `valor_imposto`, `total`, `Pagar_Imposto(v)`
- `Pessoa_Fisica : Clientes`: `cpf`, `rg` — imposto de 10% sobre o valor
- `Pessoa_Juridica : Clientes`: `cnpj`, `ie` — imposto de 20% sobre o valor (override de `Pagar_Imposto`)

## Como executar

```
dotnet run
```

O programa pede nome, endereço, tipo de cliente (`f` ou `j`), os dados
específicos (CPF/RG ou CNPJ/IE) e o valor de compra, calculando o imposto
correspondente.
