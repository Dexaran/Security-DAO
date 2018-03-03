# Ethereum Commonwealth smart-contract audit DAO.

NOTE: This is the very first implementation. It requires more testing/debugging before use.

The following describes a structure and workflow of Ethereum Commonwealth ETC & CLO smart-contract auditing department. ( read [Callisto whitepaper](https://drive.google.com/file/d/16sW_0YajCedBdLvr9jmgJqE9L-SzuYKq/view) for more information )

## Abstract

Smart-contract security is critical for most blockchain DApp development platforms. The main goal of this organization is to improve the security of Ethereum Classic and Callisto ecosystem by providing free security audits for smart-contract developers.

We do not rely on blockchain technology to verify smart-contracts. We only use it to provide a registry of audited contracts, publish and manage **results** of smart-contract audits.

It should be noted that smart-contract auditing organization is scalable which means that it allows to hire, manage and pay security audits of any smart-contracts written in any language depending on demand.

## Structure

There are two types of participants in the described organization: [managers](https://github.com/Dexaran/Security-DAO/blob/master/SecurityDAO.sol#L17) and [auditors](https://github.com/Dexaran/Security-DAO/blob/master/SecurityDAO.sol#L11-L18).

The main task of a manager is to control and verify the work of the auditors.

The main task of an auditor is to review a code of smart-contracts and submit [reports](https://github.com/Dexaran/Security-DAO/blob/master/SecurityDAO.sol#L29-L40). Auditors receive [karma](https://github.com/Dexaran/Security-DAO/blob/master/SecurityDAO.sol#L15) for reviewing contracts. They also receive [penalties](https://github.com/Dexaran/Security-DAO/blob/master/SecurityDAO.sol#L16) for making mistakes. The statistic reflects each auditors results and determines their reward.

Both, managers and auditors are paid from Callisto treasury.

The audit process will be managed through github so that it will be transparently available for everyone. A smart-contract developer should open an [issue](https://github.com/Dexaran/Security-DAO/issues) to submit his smart-contract for auditors review. Then the manager will verify security audit request details and mark the issue as *approved*. The manager should not mark dummy requests, requests that aim to spam the security audit queue or any requests that does not met coding standard requirements. After that, **every** auditor can start reviewing the code.

## Rewards

Managers are always paid regardless of their activity.
