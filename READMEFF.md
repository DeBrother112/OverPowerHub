##### This is my repository

# My name is Vova

![](https://p.turbosquid.com/ts-thumb/Qj/fHJVe4/VR/imagename/png/1687184537/1920x1080/turn_fit_q99/85b858fbfa136786300a539191d052672c841164/imagename-1.jpg)

I'm **Javascript Dev**

function redrawSortPokemons() {
    resultElement.innerHTML = ""
    sortedPokemons.forEach(pokemon => drawPokemon(pokemon))
}

document.getElementById("filter-form").addEventListener("submit", function (event) {
    event.preventDefault()
    sortedPokemons = pokemons
    if (event.target["name-filter"].value) {
        sortedPokemons = sortedPokemons.filter((pokemon) => {
            return pokemon.name.indexOf(event.target["name-filter"].value.toLowerCase()) != -1
        })
    }
    if (event.target["hp-filter-form"].value > 10) {
        sortedPokemons = sortedPokemons.filter((pokemon) => {
            return pokemon.stats[0].base_stat >= event.target["hp-filter-form"].value
        })
    }

    if (event.target["hp-filter-to"].value > 10) {
        sortedPokemons = sortedPokemons.filter((pokemon) => {
            return pokemon.stats[0].base_stat >= event.target["hp-filter-to"].value
        })
    }

    if (event.target["attack-filter-form"].value > 10) {
        sortedPokemons = sortedPokemons.filter((pokemon) => {
            return pokemon.stats[0].base_stat >= event.target["attack-filter-form"].value
        })
    }

    if (event.target["attack-filter-to"].value > 10) {
        sortedPokemons = sortedPokemons.filter((pokemon) => {
            return pokemon.stats[0].base_stat >= event.target["attack-filter-to"].value
        })
    }

    if (event.target["defence-filter-form"].value > 10) {
        sortedPokemons = sortedPokemons.filter((pokemon) => {
            return pokemon.stats[0].base_stat >= event.target["defence-filter-form"].value
        })
    }

    if (event.target["defence-filter-to"].value > 10) {
        sortedPokemons = sortedPokemons.filter((pokemon) => {
            return pokemon.stats[0].base_stat >= event.target["defence-filter-to"].value
        })
    }
    event.target['types'].forEach(function (filterType) {
        if (!filterType.checked) {
            sortedPokemons = sortedPokemons.filter(function (pokemon) {
                for (let i in pokemon.types) {
                    if (pokemon.types[i].type.name == filterType.value) return false
                }
                return true
            })
        }
    })
})

    my social links
    *[](https://www.youtube.com/watch?v=dQw4w9WgXcQ&ab_channel=RickAstley)
