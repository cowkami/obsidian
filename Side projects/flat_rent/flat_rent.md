# FlatRent

## Mission

Equal borrower and lender.

## Vision

Provide appropriate Rent fee for all.

## Use case
### Get an appropriate Rent
```mermaid
graph LR
User -->|Room info.|System
System -->|Rent|User
```

## System sequence

### Rent prediction
```mermaid
sequenceDiagram

participant Client
participant App
participant Algo

Client ->>+ App: how much is this room?
App ->>+ Algo: room info.
App -->>- Client: Wait a minuite.
Algo ->>- App: Rent prediction
App ->> Client: Rent prediction
```
### Update model


```mermaid
sequenceDiagram

participant Algo
participant DB for Algo
participant Scraper

loop Scraping and Update model
  Scraper ->> DB for Algo: Room data
  Algo ->> DB for Algo: Query room data
  DB for Algo ->> Algo: Room data
end
```


### Rent prediction

## Features

### Priority

- Rent prediction: Room info. -> Rent

### in-Priority

- Room prediction: Rent -> Place -> Room info.

## Cost
- Server maintanance fee

