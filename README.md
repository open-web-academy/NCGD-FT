### Example-Token

ID=dev-1653521107679-88908214949697

Inicializar contrato

    near call $ID init_contract '{"owner_id": "yairnava.testnet"}' --accountId $ID

Obtener propietario del contrato
    
    near view $ID get_owner_id


Cambiar propietario del contrato

    near call $ID set_owner_id '{"owner_id": "yairnh.testnet"}' --accountId yairnava.testnet

Obtener lista de mineros
    
    near view $ID get_minters

Agregar minero

    near call $ID add_minter '{"account_id": "yairnh.testnet"}' --accountId yairnava.testnet

Remover minero

    near call $ID remove_minter '{"account_id": "yairnh.testnet"}' --accountId yairnava.testnet

Minar FT Token

    near call $ID mint '{"account_id": "yairnava.testnet", "amount" : "100000000000000000000000000000000"}' --accountId yairnava.testnet

Obtener balance total de STRW-Token
    
    near view $ID ft_total_supply

Obtener balance de una cuenta de STRW-Token

    near view $ID ft_balance_of '{"account_id": "yairnava.testnet"}'

Mostrar STRW-Token en Wallet

    near call $ID ft_transfer '{"receiver_id": "yairnava.testnet", "amount":"0", "memo":""}' --accountId yairnava.testnet