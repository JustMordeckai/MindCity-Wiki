# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Testing Function

```lua
    Citizen.CreateThread(function()
        while true do
            if ESX.PlayerData.job and ESX.PlayerData.job.name == 'gouv' then
                if IsControlJustPressed(1,167) then
                    OpenMenu('gouvf6', 'main')
                end
            else
                Citizen.Wait(5000)
            end

            Citizen.Wait(2)
        end
    end)
```

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
