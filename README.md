
# Catálogo de Vídeos

## Video 1
- Título: Aventura na Floresta
- Descrição: Um filme sobre uma jornada épica na selva.
- Ano: 2024
- Duração: 120 minutos
- Gênero: Ação, Aventura

## Video 2
- Título: Mistérios do Mar
- Descrição: Documentário sobre os oceanos do planeta.
- Ano: 2023
- Duração: 90 minutos
- Gênero: Documentário
git add catalogo.md
git commit -m "Atualizar catálogo de vídeos com novos títulos"
git push origin main
import json

# Dados do catálogo
catalogo = {
    "videos": [
        {
            "titulo": "Aventura na Floresta",
            "descricao": "Um filme sobre uma jornada épica na selva.",
            "ano": 2024,
            "duracao": "120 minutos",
            "genero": ["Ação", "Aventura"]
        },
        {
            "titulo": "Mistérios do Mar",
            "descricao": "Documentário sobre os oceanos do planeta.",
            "ano": 2023,
            "duracao": "90 minutos",
            "genero": ["Documentário"]
        }
    ]
}

# Escrever no arquivo JSON
with open('catalogo.json', 'w') as f:
    json.dump(catalogo, f, indent=4)

print("Catálogo atualizado com sucesso!")
