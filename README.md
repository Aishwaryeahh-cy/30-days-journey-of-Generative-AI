<!--
  README.md — Generative AI ✨
  Paste this single file into your repo root as README.md
  The 3D banner below is pure inline SVG (no external JS/CSS), so it animates on GitHub.
-->

<p align="center">
  <!-- 3D-ish animated SVG banner -->
  <svg width="100%" viewBox="0 0 1200 360" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Generative AI">
    <defs>
      <!-- Soft glow -->
      <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
        <feGaussianBlur stdDeviation="6" result="coloredBlur"/>
        <feMerge>
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>

      <!-- Moving gradient for text -->
      <linearGradient id="grad" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%"  stop-color="#7C3AED"/>
        <stop offset="50%" stop-color="#06B6D4"/>
        <stop offset="100%" stop-color="#22C55E"/>
        <animate attributeName="x1" values="0%;100%;0%" dur="8s" repeatCount="indefinite"/>
        <animate attributeName="x2" values="100%;0%;100%" dur="8s" repeatCount="indefinite"/>
      </linearGradient>

      <!-- Floor grid pattern -->
      <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
        <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#2f2f39" stroke-width="1"/>
      </pattern>

      <!-- 3D cube faces -->
      <linearGradient id="faceA" x1="0" y1="0" x2="1" y2="1">
        <stop offset="0%" stop-color="#0ea5e9"/>
        <stop offset="100%" stop-color="#7c3aed"/>
      </linearGradient>
      <linearGradient id="faceB" x1="1" y1="0" x2="0" y2="1">
        <stop offset="0%" stop-color="#22c55e"/>
        <stop offset="100%" stop-color="#06b6d4"/>
      </linearGradient>
      <linearGradient id="faceC" x1="0" y1="1" x2="1" y2="0">
        <stop offset="0%" stop-color="#f59e0b"/>
        <stop offset="100%" stop-color="#ef4444"/>
      </linearGradient>
    </defs>

    <!-- Background -->
    <rect x="0" y="0" width="1200" height="360" fill="#0b0b12"/>
    <rect x="0" y="240" width="1200" height="120" fill="url(#grid)" opacity="0.5"/>

    <!-- Floating particles -->
    <g opacity="0.5">
      <circle cx="150" cy="80" r="2" fill="#22C55E">
        <animate attributeName="cy" values="80;70;80" dur="6s" repeatCount="indefinite"/>
      </circle>
      <circle cx="1080" cy="60" r="2" fill="#06B6D4">
        <animate attributeName="cy" values="60;48;60" dur="7s" repeatCount="indefinite"/>
      </circle>
      <circle cx="950" cy="120" r="2" fill="#7C3AED">
        <animate attributeName="cy" values="120;108;120" dur="5.5s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- Rotating 3D cube -->
    <g transform="translate(260,180) scale(1.2)" filter="url(#glow)">
      <g>
        <!-- Use animateTransform (SMIL) so it runs on GitHub -->
        <g>
          <g>
            <!-- Group for rotation -->
            <g>
              <g>
                <g>
                  <g>
                    <g>
                      <g>
                        <g>
                          <g>
                            <g>
                              <g>
                                <g>
                                  <g>
                                    <g>
                                      <g>
                                        <g>
                                          <g>
                                            <g>
                                              <g>
                                                <g>
                                                  <g>
                                                    <g>
                                                      <g>
                                                        <g>
                                                          <g>
                                                            <g>
                                                              <g>
                                                                <g>
                                                                  <g>
                                                                    <g>
                                                                      <g>
                                                                        <g>
                                                                          <g>
                                                                            <g>
                                                                              <g>
                                                                                <g>
                                                                                  <g>
                                                                                    <g>
                                                                                      <g>
                                                                                        <g>
                                                                                          <g>
                                                                                            <!-- Faces of an isometric cube -->
                                                                                            <g id="cube">
                                                                                              <!-- Right face -->
                                                                                              <polygon points="60,-100 160,-40 160,60 60,0"
                                                                                                       fill="url(#faceA)" opacity="0.95"/>
                                                                                              <!-- Left face -->
                                                                                              <polygon points="-140,-40 -40,-100 60,-40 60,60 -40,120 -140,60"
                                                                                                       fill="url(#faceB)" opacity="0.95"/>
                                                                                              <!-- Top face -->
                                                                                              <polygon points="-40,-100 60,-160 160,-100 60,-40"
                                                                                                       fill="url(#faceC)" opacity="0.95"/>
                                                                                            </g>
                                                                                            <animateTransform attributeName="transform"
                                                                                                              attributeType="XML"
                                                                                                              type="rotate"
                                                                                                              from="0 10 -40"
                                                                                                              to="360 10 -40"
                                                                                                              dur="14s"
                                                                                                              repeatCount="indefinite"/>
                                                                                          </g>
                                                                                        </g>
                                                                                      </g>
                                                                                    </g>
                                                                                  </g>
                                                                                </g>
                                                                              </g>
                                                                            </g>
                                                                          </g>
                                                                        </g>
                                                                      </g>
                                                                    </g>
                                                                  </g>
                                                                </g>
                                                              </g>
                                                            </g>
                                                          </g>
                                                        </g>
                                                      </g>
                                                    </g>
                                                  </g>
                                                </g>
                                              </g>
                                            </g>
                                          </g>
                                        </g>
                                      </g>
                                    </g>
                                  </g>
                                </g>
                              </g>
                            </g>
                          </g>
                        </g>
                      </g>
                    </g>
                  </g>
                </g>
              </g>
            </g>
          </g>
        </g>
      </g>
    </g>

    <!-- Animated headline -->
    <g transform="translate(520,190)" filter="url(#glow)">
      <text x="0" y="-10" font-family="Poppins, Segoe UI, Roboto, Arial, sans-serif"
            font-size="64" font-weight="800" fill="url(#grad)" letter-spacing="2">
        GENERATIVE&nbsp;AI
        <animate attributeName="letter-spacing" values="2;6;2" dur="6s" repeatCount="indefinite"/>
      </text>
      <text x="0" y="36" font-family="Inter, Segoe UI, Roboto, Arial, sans-serif"
            font-size="20" fill="#c7d2fe" opacity="0.9">
        Models that write, draw, compose, and code.
        <animate attributeName="opacity" values="0.6;1;0.6" dur="6s" repeatCount="indefinite"/>
      </text>
    </g>
  </svg>
</p>

<h1 align="center">🚀 Generative AI – The Fun, Fast Starter Repo</h1>
<p align="center">
  <em>Text · Images · Code · Audio — all generated by models you control.</em>
</p>

<p align="center">
  <a href="#quickstart">Quickstart</a> •
  <a href="#features">Features</a> •
  <a href="#examples">Examples</a> •
  <a href="#faq">FAQ</a>
</p>

---

## ✨ Why This Repo?
- **One place** to try text, image, and code generation.
- **Beginner-friendly** scripts with sensible defaults.
- **No vendor lock-in** — swap models (OpenAI, local, etc.).

---

## 🔧 Quickstart

> **Option A (Python)**
```bash
# 1) Create env
python -m venv .venv && source .venv/bin/activate  # on Windows use: .venv\Scripts\activate
pip install -U pip

# 2) Install core deps (feel free to replace openai with any client you prefer)
pip install openai pillow numpy

# 3) Set your key (example: OpenAI; or use your chosen provider)
export OPENAI_API_KEY="YOUR_KEY_HERE"  # PowerShell: setx OPENAI_API_KEY "YOUR_KEY_HERE"
