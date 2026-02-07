Definitions
Copy code

λ_γ  = photon wavelength
L_shell(s) = shell coherence scale (e.g., resonance domain size)
Mean Deflection
Copy code

⟨α⟩ ≈ ∫₀^S λ(s) · ⟨θ_scatter⟩ ds
Deflection Variance
Copy code

σ_α² ≈ ∫₀^S λ(s) · σ_θ²(s) ds
Stochastic Small-Angle Diffusion (Fokker-Planck)
Copy code

d⟨θ²⟩ / ds = λ(s) · σ_θ²(s)
with
Copy code

σ_θ²(s) ∝ ( λ_γ / L_shell(s) )²
Interaction Rate and Optical Depth (Master Integral)
Copy code

λ(s) = κ_EMN(s) · ρ_shell(s) · ℛ
Copy code

τ(s) = ∫₀^s λ(s′) ds′
This τ controls deflection, redshift, dimming, and delay.
Frequency Evolution (Refinement B: Path-Dependent δ)
Per absorption–re-emission
Copy code

δ(s) = τ_chrono · [ κ_EMN(s) / κ_EMN_ref ]
where
Copy code

κ_EMN_ref = reference curvature (e.g., vacuum or average value)
Redshift Integral
Copy code

z ≈ ∫₀^S δ(s) · A · λ(s) ds
Substitute λ(s):
Copy code

z = A · τ_chrono · ∫₀^S [ κ_EMN(s) / κ_EMN_ref ] · λ(s) ds
Expand:
Copy code

z = A · τ_chrono · ∫₀^S [ κ_EMN²(s) · ρ_shell(s) · ℛ / κ_EMN_ref ] ds
Exact form (non-small-z):
Copy code

z = exp( ∫ δ(s) · A · λ(s) ds ) − 1
Direction Evolution (Hybrid Deterministic + Stochastic)
Ballistic regions
Copy code

d n̂ / ds = 0
Deterministic shell interaction
Copy code

n̂′ = n̂ − 2 ( n̂ · n̂_b ) n̂_b
or
Copy code

n̂′ ≈ n̂ + Δθ
(depending on shell geometry)
Stochastic diffusion (variance)
Copy code

σ_α² ≈ ∫₀^S λ(s) · σ_θ²(s) ds
Copy code

σ_α² ∝ ∫₀^S λ(s) · ( λ_γ / L_shell(s) )² ds
Intensity and Delay (Unchanged Structure)
Dimming
Copy code

I_out ≈ I_0 [ exp(−τ) + f (1 − exp(−τ)) g(Δθ) ]
Delay
Copy code

Δt ≈ A · τ · ( τ_chrono / ρ_shell )
Quick Math Check (Constant-Parameter Approximation)
Assuming constants for symbolic check:
Copy code

z = ( κ_EMN² · ℛ · ρ_shell · S · τ_chrono ) / κ_EMN_ref
This matches the quadratic κ_EMN dependence.
Key Scaling Relations
Copy code

⟨α⟩ ∝ ∫ κ_EMN · ρ_shell · ℛ ds
Copy code

z ∝ ∫ κ_EMN² · ρ_shell · ℛ ds
Copy code

σ_α² ∝ λ_γ²
Thin Spherical Shell Toy Model
Assume:
Copy code

κ_EMN(r) = κ₀ ( r₀ / r )
ρ_shell(r) = ρ₀ ( r₀ / r )
ℛ = 1
Path length:
Copy code

S ≈ 2 √( R² − b² )
Thin-shell optical depth:
Copy code

τ ≈ λ · d
Deflection:
Copy code

⟨α⟩ ≈ ( R + T ) · ( κ₀ ρ₀ r₀² / R² ) · d · θ₀
Redshift:
Copy code

z ≈ A · τ_chrono · ( κ₀² ρ₀ r₀² / ( R² κ_ref ) ) · d
Discriminator
Copy code

z / α ∝ κ₀
UQLT predicts growth of z relative to α in strong-κ regions.
GR predicts a constant ratio.
