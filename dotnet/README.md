# Dotnet Action

## Dotnet Build

```console
      - uses: artdolya/actions/dotnet@master
```

## Dotnet Build and run Tests

```console
      - uses: artdolya/actions/dotnet@master
        with:
          work-dir: ./src/Net
          dotnet-version: 8.x
          run-tests: true
```

## Dotnet Build and publish to Nuget

```console
      - uses: artdolya/actions/dotnet@master
        with:
          work-dir: ./src/Net/Data/KrapkaNet.Data.Abstractions
          dotnet-version: 8.x
          nuget-api-key: ${{ secrets.NUGET_API_KEY }} ## Should not be null
```

