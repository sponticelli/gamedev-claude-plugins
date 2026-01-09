---
name: web-optimization-checklist
description: Generate optimization checklist for web game release
---

# Web Game Optimization Checklist

Generate a comprehensive optimization checklist for releasing a web game.

## Checklist Categories

### Build Optimization
### Asset Optimization
### Runtime Performance
### Loading Performance
### Mobile Optimization

## Output Format

```markdown
# Web Game Release Optimization Checklist: [Game Name]

## Build Optimization

### JavaScript
- [ ] Code minified (Terser/esbuild)
- [ ] Tree shaking enabled
- [ ] Dead code eliminated
- [ ] Source maps generated (but not deployed to prod)
- [ ] Chunks split appropriately
- [ ] Critical path JS inlined or preloaded

### CSS
- [ ] CSS minified
- [ ] Unused CSS removed (PurgeCSS)
- [ ] Critical CSS inlined
- [ ] Non-critical CSS deferred

### Bundle Analysis
- [ ] Bundle size analyzed (webpack-bundle-analyzer or similar)
- [ ] Large dependencies identified
- [ ] Tree-shakeable alternatives considered
- [ ] Total JS < [target] KB (gzipped)

---

## Asset Optimization

### Images/Textures
- [ ] Images compressed (TinyPNG, ImageOptim)
- [ ] Appropriate formats used (WebP with fallback)
- [ ] Texture atlases created
- [ ] Mipmaps generated where needed
- [ ] Power-of-two textures (for WebGL)
- [ ] Resolution appropriate for use (no 4K for thumbnails)

### Audio
- [ ] Audio compressed appropriately
- [ ] Multiple formats provided (MP3 + OGG/WebM)
- [ ] Audio sprites created for SFX
- [ ] Streaming for long audio files
- [ ] Bit rate appropriate (128kbps for music, lower for SFX)

### Fonts
- [ ] Font subset to used characters
- [ ] WOFF2 format used
- [ ] font-display: swap configured
- [ ] Fallback fonts specified

### 3D Assets (if applicable)
- [ ] Models optimized (polycount)
- [ ] Textures compressed (Basis/KTX2)
- [ ] GLB over GLTF (binary is smaller)
- [ ] Draco compression for geometry

---

## Runtime Performance

### Frame Rate
- [ ] 60 FPS on desktop targets
- [ ] 30+ FPS on mobile targets
- [ ] No regular frame drops/stutters
- [ ] requestAnimationFrame used (not setInterval)

### Memory
- [ ] Object pooling implemented
- [ ] No per-frame allocations in hot paths
- [ ] GC pauses < 16ms
- [ ] Memory stable over long sessions
- [ ] Cleanup on scene/level transitions

### Rendering
- [ ] Draw calls minimized (batching)
- [ ] Overdraw reduced
- [ ] Culling implemented
- [ ] LOD system (for complex 3D)

### JavaScript
- [ ] Hot paths profiled and optimized
- [ ] No blocking operations in render loop
- [ ] Web Workers for heavy computation
- [ ] TypedArrays for numeric data

---

## Loading Performance

### Initial Load
- [ ] First Contentful Paint < 1.5s
- [ ] Time to Interactive < 3s
- [ ] Largest Contentful Paint < 2.5s
- [ ] Loading screen appears quickly

### Asset Loading
- [ ] Progressive loading implemented
- [ ] Critical assets preloaded
- [ ] Non-critical assets deferred
- [ ] Loading progress displayed
- [ ] Retry logic for failed loads

### Caching
- [ ] Cache headers configured
- [ ] Service worker caching (PWA)
- [ ] Asset versioning (cache busting)
- [ ] Repeat visits fast

### Network
- [ ] HTTP/2 enabled
- [ ] Gzip/Brotli compression
- [ ] CDN for static assets
- [ ] DNS prefetch for external domains

---

## Mobile Optimization

### Touch
- [ ] Touch targets >= 48px
- [ ] No hover-dependent interactions
- [ ] Touch feedback visible
- [ ] Gestures intuitive

### Display
- [ ] Responsive design works
- [ ] Orientation changes handled
- [ ] Safe area insets respected (notch)
- [ ] High DPI handled correctly

### Performance
- [ ] Reduced effects on mobile
- [ ] Lower resolution option
- [ ] Battery-conscious (no unnecessary work)
- [ ] Thermal throttling tested

### Connectivity
- [ ] Works on slow connections
- [ ] Offline mode (if PWA)
- [ ] Low data mode (reduced assets)

---

## PWA Checklist (if applicable)

- [ ] Manifest valid
- [ ] Service worker registered
- [ ] Icons all sizes
- [ ] Offline experience defined
- [ ] Install prompt appropriate
- [ ] Updates handled gracefully

---

## Pre-Launch Verification

### Cross-Browser
- [ ] Chrome desktop: tested
- [ ] Firefox desktop: tested
- [ ] Safari desktop: tested
- [ ] Chrome Android: tested
- [ ] Safari iOS: tested

### Analytics
- [ ] Performance monitoring setup
- [ ] Error tracking enabled
- [ ] Load time tracking
- [ ] Core Web Vitals monitored

### Final Checks
- [ ] Console free of errors/warnings
- [ ] No debug code in production
- [ ] Source maps separate (not in bundle)
- [ ] Production environment vars set

---

## Performance Budget

| Metric | Budget | Actual | Status |
|--------|--------|--------|--------|
| Total JS (gzipped) | < [X] KB | [X] KB | [✓/✗] |
| Total CSS (gzipped) | < [X] KB | [X] KB | [✓/✗] |
| Total Assets | < [X] MB | [X] MB | [✓/✗] |
| Initial Load | < [X] s | [X] s | [✓/✗] |
| Frame Time (desktop) | < 16 ms | [X] ms | [✓/✗] |
| Frame Time (mobile) | < 33 ms | [X] ms | [✓/✗] |
| Memory (steady state) | < [X] MB | [X] MB | [✓/✗] |
```

Generate the checklist customized for the specific game and platform requirements.
