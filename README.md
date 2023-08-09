<h1 align="center">perlin2d</h1>
<div align="center">

  <img alt="GitHub" src="https://img.shields.io/github/license/gp-97/perlin">

</div>
<div align="center">
  
  [![Status](https://img.shields.io/badge/status-active-success.svg)]()
  [![GitHub Issues](https://img.shields.io/github/issues/gp-97/perlin2d.svg)](https://github.com/gp-97/perlin2d/issues)
  [![GitHub Pull Requests](https://img.shields.io/github/issues-pr/gp-97/perlin2d.svg)](https://github.com/gp-97/perlin2d/pulls)
  ![Crates.io (recent)](https://img.shields.io/crates/dr/perlin2d?style=plastic)
  ![Github Workflow](https://github.com/gp-97/perlin2d/actions/workflows/main.yml/badge.svg)

</div>

---
A small, fast and efficient two dimensional Perlin noise generation library with zero dependencies.

`#![no_std]` support available on nightly with `default-features = false`.

- [Documentation](https://docs.rs/perlin2d/0.2.5/perlin2d/)
- [crate.io](https://crates.io/crates/perlin2d)

### Example usage
```rust
  // For example, to generate a Perlin noise 2D terrain:
  use perlin2d::PerlinNoise2D;

  let perlin = PerlinNoise2D::new(6, 10.0, 0.5, 1.0, 2.0, (100.0, 100.0), 0.5, 101);
  let noise = perlin.get_noise(5.0, 10.0);
```
