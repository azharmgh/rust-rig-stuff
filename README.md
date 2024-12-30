# rust-rig-stuff



[medium article](https://medium.com/@0thTachi/build-a-flight-search-ai-agent-with-rust-using-rig-f93539c7337a)

[github source](https://github.com/0xPlaygrounds/rig-examples/tree/main/flight_search_assistant)


```
cargo new flight_search_assistant
cd flight_search_assistant
```


update the cargo.toml file

```

[package]
name = "flight_search_assistant"
version = "0.1.0"
edition = "2024"


[dependencies]
rig-core = "0.1.0"
tokio = { version = "1.34.0", features = ["full"] }
anyhow = "1.0.75"
serde = { version = "1.0", features = ["derive"] }
serde_json = "1.0"
reqwest = { version = "0.11", features = ["json"] }
dotenv = "0.15"
async-trait = "0.1"
thiserror = "1.0"
chrono = { version = "0.4", features = ["serde"] }


```


add keys to the .env file

```
OPENAI_API_KEY=mykey
RAPIDAPI_KEY=myrkey

```

run ```cargo build```

touch ``` src/flight_search_tool.rs```

