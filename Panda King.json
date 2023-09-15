SELECT
    sender AS address,
    COUNT(evt_tx_hash) AS tx_count
FROM (
    SELECT 
        contract_address,
        evt_tx_hash,
        sender
    FROM polyhedra_network_bnb.NFTBridgeImplementation_evt_TransferNFT
    WHERE
        token <> 0xD2cCC9EE7Ea2ccd154c727A46D475ddA49E99852 AND
        token <> 0x9c614a8E5a23725214024d2C3633BE30D44806f9 AND
        token <> 0x9885C17Dd44c00C37B98F510cdff099EfF437dcE AND
        token <> 0xC5ae0d15593316e0cC905840eD2dE83E2DD4EA9E AND
        token <> 0x13D23d867e73aF912Adf5d5bd47915261eFa28F2 AND
        token <> 0x9e8C1e7B35f646A606644a5532C6103C647938cf AND
        token <> 0x40a2A882c82AD7cC74E5f58Cde7612c07956D4A6
    UNION ALL 
  
    
    SELECT 
        contract_address,
        evt_tx_hash,
        sender
    FROM nft_bridge_bnb.NFT721Bridge_evt_TransferNFT
    WHERE
        token <> 0xD2cCC9EE7Ea2ccd154c727A46D475ddA49E99852 AND
        token <> 0x9c614a8E5a23725214024d2C3633BE30D44806f9 AND
        token <> 0x9885C17Dd44c00C37B98F510cdff099EfF437dcE AND
        token <> 0xC5ae0d15593316e0cC905840eD2dE83E2DD4EA9E AND
        token <> 0x13D23d867e73aF912Adf5d5bd47915261eFa28F2 AND
        token <> 0x9e8C1e7B35f646A606644a5532C6103C647938cf AND
        token <> 0x40a2A882c82AD7cC74E5f58Cde7612c07956D4A6
    UNION ALL 
    
    
    SELECT 
        contract_address,
        evt_tx_hash,
        sender
    FROM polyhendra_pandra_polygon.NFT721Bridge_evt_TransferNFT
    WHERE
        token <> 0xfeb105763753e9d26DfD4aae1Ed368aa7cC18260 AND
        token <> 0x6b0C248679F493481411a0A14cd5FC2DBBe8Ab02 AND
        token <> 0x9d5d479a84f3358e8e27afe056494bd2da239acd
    UNION ALL 
    
    
    SELECT 
        contract_address,
        evt_tx_hash,
        sender
    FROM polyhedra_pandra_no_l0_test_network_polygon.NFTBridgeImplementation_evt_TransferNFT
    WHERE
        token <> 0xfeb105763753e9d26DfD4aae1Ed368aa7cC18260 AND
        token <> 0x6b0C248679F493481411a0A14cd5FC2DBBe8Ab02 AND
        token <> 0x9d5d479a84f3358e8e27afe056494bd2da239acd
    UNION ALL
    
    
    SELECT 
        contract_address,
        evt_tx_hash,
        sender
    FROM polyhedra_pandra_celo_l0_celo.NFT721Bridge_evt_TransferNFT
    UNION ALL 
    
    SELECT 
        contract_address,
        evt_tx_hash,
        sender
    FROM polyhedra_pandra_celo_no_l0_celo.NFTBridgeImplementation_evt_TransferNFT
) AS combined_data
GROUP BY sender;
