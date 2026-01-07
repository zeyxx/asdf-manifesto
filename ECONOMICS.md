# Economics

The economic model of $asdfasdfa is radical in its simplicity: **100% of fees burn.**

## The One Rule

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│                         EVERY FEE → 100% BURN                           │
│                                                                         │
│   No treasury allocation.                                               │
│   No team percentage.                                                   │
│   No VC unlock schedule.                                                │
│   No governance extraction.                                             │
│                                                                         │
│   Just burn.                                                            │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

## Supply Dynamics

### The Math

```
Supply(t+1) = Supply(t) - Burns(t)

Where Burns(t) = Σ(fees from all ecosystem interactions)
```

### Asymptotic Deflation

```
                    Supply
                       │
Initial Supply ────────┤
                       │╲
                       │ ╲
                       │  ╲
                       │   ╲
                       │    ╲
                       │     ╲____
                       │          ╲____
                       │               ╲________
                       │                        ╲____________
                       └────────────────────────────────────────→ Time

Supply approaches 0 asymptotically but never reaches 0.
Decimals allow infinite subdivision.
```

### Value Per Token

```
As Supply ↓ and Demand constant or ↑:

Value per token = Total Demand / Circulating Supply

With burns: Value per token ↑ over time
Traditional: Value per token ↓ over time (inflation)
```

## Comparison Models

### Traditional Extractive Model

```
FEE FLOW:
User pays fee → Platform takes 100% → Shareholders profit
                                           │
                                           ↓
                                    Value EXITS system
                                           │
                                           ↓
                                    Users = Product
```

### Partial Burn Model (e.g., ETH post-merge)

```
FEE FLOW:
User pays fee ─┬─→ Base fee burns (~50%)
               │
               └─→ Priority fee → Validators (~50%)
                                        │
                                        ↓
                                 Partial extraction
```

### $asdfasdfa Model

```
FEE FLOW:
User pays fee → 100% BURN → Supply ↓ → All holders benefit
                                            │
                                            ↓
                                     Value STAYS in system
                                            │
                                            ↓
                                     Users = Owners (if hold)
```

## Incentive Alignment

### The Matrix

| Actor | Extractive System | $asdfasdfa System |
|-------|-------------------|-------------------|
| **Trader** | Pays fees, enriches platform | Pays fees, burns, hold appreciates |
| **Holder** | Diluted by inflation/unlocks | Burns compound value |
| **Builder** | Works for equity/salary | Builds → usage → burns → hold ↑ |
| **User** | Is the product | Is an owner (if holds) |
| **Platform** | Extracts maximum | Doesn't exist (protocol only) |

### Why It Works

```
Traditional incentive conflict:
Platform wants: Maximum extraction
Users want: Minimum fees
Result: Adversarial relationship

$asdfasdfa incentive alignment:
Protocol wants: Maximum usage (= maximum burns)
Users want: Maximum value (= maximum burns)
Holders want: Maximum burns
Builders want: Maximum usage (= maximum burns)
Result: Everyone optimizes for the same thing
```

## Burn Sources

### Current

| Source | Trigger | Burn |
|--------|---------|------|
| GASdf | Any transaction via gas abstraction | 100% |
| HolDex | API queries, premium features | 100% |
| Ignition | Token launches | 100% |
| ASDForecast | Prediction fees | 100% |

### Future

| Source | Trigger | Burn |
|--------|---------|------|
| Trading app | Trades | 100% |
| Social app | Premium features | 100% |
| Bridge | Cross-chain transfers | 100% |
| Any new app | Any fee | 100% |

## Cross-Token Burns

### The Mechanism

When a user pays fees in a token other than $asdfasdfa:

```
1. User pays fee in Token X (SOL, USDC, any token)
         │
         ↓
2. Token X is swapped to $asdfasdfa
         │
         ↓
3. $asdfasdfa is burned
         │
         ↓
4. Supply decreases
```

### Implications

- **Any token can pay for burns**: SOL, USDC, memecoins
- **Market buy pressure**: Every fee creates buy pressure before burn
- **Universal deflation**: Even users who never hold $asdfasdfa contribute to burns
- **Ecosystem tax**: Using any ecosystem app = burning $asdfasdfa

## Internal Ratios

While the burn is 100%, internal measurements use φ (phi) proportions for consistency:

```
φ = 1.618033988749895
φ⁻¹ = 61.8%
φ⁻² = 38.2%
```

These ratios guide thresholds and weights. They could be different numbers. We chose φ for aesthetic consistency across the system, not for any mystical properties.

### K-Score Formula

```
K = 100 × ∛(D × O × L)

Geometric mean ensures:
- No single metric can compensate for failure in another
- Balance is rewarded
- Extremes are punished
```

## Anti-Ponzi Properties

### Traditional Token (Ponzi-like)

```
Timeline:
T0: Early buyers buy cheap
T1: Marketing creates hype
T2: New buyers buy at higher price
T3: Early buyers sell to new buyers
T4: Music stops, late buyers hold bags

Value flow: Later buyers → Earlier buyers
Sustainability: Requires constant new money
```

### $asdfasdfa (Non-Ponzi)

```
Timeline:
T0: Buyers acquire tokens
T1: Ecosystem generates usage
T2: Usage generates burns
T3: Burns reduce supply
T4: All holders benefit equally from burns

Value flow: Usage → All holders (proportionally)
Sustainability: Requires usage, not new buyers
```

### Key Difference

```
Ponzi:      New money funds old holders
$asdfasdfa: Activity funds all holders

A holder from day 1 and a holder from day 1000
benefit EQUALLY from the same burn.
No early-adopter extraction.
```

## Funding Development

### The Question

> "If 100% burns, how do you fund development?"

### The Answer

**Builders are holders.**

```
Traditional:
Builder → Works for company → Gets salary → Company extracts fees

$asdfasdfa:
Builder → Holds tokens → Builds ecosystem → Usage increases
                                                    │
                                                    ↓
                                           Burns increase
                                                    │
                                                    ↓
                                           Hold value increases
                                                    │
                                                    ↓
                                           Builder rewarded
```

### Why It's Sustainable

1. **Aligned incentives**: Builder success = ecosystem success = holder success
2. **No extraction overhead**: 0% to "company" means more burns, more value
3. **Self-selecting**: Only builders who believe in the model participate
4. **Long-term thinking**: Hold incentivizes building for durability, not quick extraction

## Economic Moat

### "Anyone can fork and remove the burn"

True. But consider:

1. **Network effects don't fork**
   - K-Score needs data
   - Data needs users
   - Users need K-Score
   - Fork starts with 0 data

2. **Liquidity doesn't fork**
   - Pools have depth
   - Fork pools start at 0
   - No liquidity = no trades

3. **Builders don't fork**
   - If you build on fork, you compete with original
   - If you build on original, you benefit from existing burns
   - Rational choice: build on original

4. **If fork extracts**
   - Users prefer non-extractive original
   - Fork bleeds users back to original

5. **If fork also burns**
   - Validates the model
   - May even increase awareness of original
   - Competition is fine

## Long-Term Dynamics

The model predicts three phases if adoption continues:

**Accumulation:** Ecosystem apps launch. Burns begin compounding. Network effects establish. Builder community forms.

**Maturation:** GASdf and K-Score gain adoption. Burns reach significant volume. Supply contracts.

**Equilibrium:** Ecosystem becomes infrastructure. Burns steady. Supply stabilizes at lower level.

We're not predicting when these phases occur—only that the model tends toward this progression with continued usage.

## Mathematical Model

### Simplified Burn Model

```
Let:
- S(0) = Initial supply
- B = Burns per period
- S(t) = Supply at time t

S(t) = S(0) - B × t

Until minimum supply threshold (accounting for lost tokens, etc.)
```

### With Variable Burn Rate

```
Let:
- U(t) = Usage at time t
- f = Fee rate
- B(t) = U(t) × f

S(t) = S(0) - ∫₀ᵗ B(τ) dτ

As ecosystem grows, U(t) increases, B(t) increases, S(t) decreases faster.
```

### Value Model

```
Let:
- V(t) = Value per token at time t
- D(t) = Total demand at time t
- S(t) = Supply at time t

V(t) = D(t) / S(t)

With:
- D(t) growing (more utility, more users)
- S(t) shrinking (burns)

V(t) increases from both numerator AND denominator effects.
```

## Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│                         ECONOMIC PRINCIPLES                              │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  1. BURN EVERYTHING                                                     │
│     100% of fees → burn                                                 │
│     No extraction at any level                                          │
│                                                                         │
│  2. ALIGN EVERYONE                                                      │
│     All actors optimize for same goal: usage                            │
│     No adversarial relationships                                        │
│                                                                         │
│  3. TIME AS ALLY                                                        │
│     Deflation rewards patience                                          │
│     Longer hold = more burns accumulated                                │
│                                                                         │
│  4. USAGE AS VALUE                                                      │
│     Every interaction = burn = value                                    │
│     Utility drives economics, not speculation                           │
│                                                                         │
│  5. SIMPLICITY AS MOAT                                                  │
│     One rule: burn everything                                           │
│     No complex tokenomics to game                                       │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

*The economics are simple. The implications are profound. This is fine.*
