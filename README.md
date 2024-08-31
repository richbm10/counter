#Starknet Counter
This is an onboarding project in Cairo Language to new Starknet smart contract developers.

## Environment
* scarb 2.6.5
* cairo 2.6.4
* sierra 1.5.0
* starknet-devnet 0.1.2
* starkli 0.3.4

## Declare Class

```starkli declare target/dev/counter_CounterContract.contract_class.json --rpc http://0.0.0.0:5050 --account .c-wallets/account0_account.json --keystore .c-wallets/account0_keystore.json```

<img width="1512" alt="Screenshot 2024-08-31 at 00 17 31" src="https://github.com/user-attachments/assets/65ba33f1-a426-47ef-9b6c-f8071386e893">

## Deploy Contract

```starkli deploy --rpc http://0.0.0.0:5050 --account .c-wallets/account0_account.json --keystore .c-wallets/account0_keystore.json 0x0275e2ae49fa8b38d72284fa3d0aab444a9c44a24858b7d4c332d2d94cce14a3 0x12```

<img width="1510" alt="Screenshot 2024-08-31 at 00 18 10" src="https://github.com/user-attachments/assets/581cd3a8-e1d1-4f16-96f2-e6b9a166e4db">

## Test Counter

```starkli call --rpc http://0.0.0.0:5050 0x0618b267f5138d306861ffb4c4d780bbf271796671fc94ced23e5d4483fecf1e get_counter```

<img width="1511" alt="Screenshot 2024-08-31 at 00 18 50" src="https://github.com/user-attachments/assets/11c834cb-e495-469a-915d-e5a7c77322bb">
