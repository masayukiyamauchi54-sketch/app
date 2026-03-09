<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <title>Quantum Geometry Lecture App</title>
    <style>
        body { margin: 0; background: #050505; color: white; font-family: 'Helvetica Neue', Arial, sans-serif; overflow: hidden; }
        #ui { position: absolute; top: 20px; left: 20px; width: 350px; background: rgba(0,0,0,0.8); padding: 20px; border-radius: 15px; border: 1px solid #444; pointer-events: auto; }
        h1 { font-size: 1.2em; color: #00d4ff; margin-top: 0; }
        .step-desc { font-size: 0.9em; line-height: 1.6; color: #ccc; margin-bottom: 20px; }
        .controls { display: flex; flex-direction: column; gap: 10px; }
        label { font-size: 0.8em; color: #888; }
        button { background: #00d4ff; border: none; padding: 10px; border-radius: 5px; cursor: pointer; font-weight: bold; transition: 0.3s; }
        button:hover { background: #0099ff; }
        canvas { display: block; }
        #status { position: absolute; bottom: 20px; left: 20px; font-size: 0.8em; color: #666; }
    </style>
</head>
<body>

<div id="ui">
    <h1 id="title">量子幾何学レクチャー</h1>
    <div id="description" class="step-desc">
        まずは最小の立体「正四面体」から始めましょう。頂点が「虚軸（4次元）」、底面が「実軸（3次元）」です。
    </div>
    <div class="controls">
        <button onclick="nextStep()">次のフェーズへ進む</button>
        <label>スピン速度</label>
        <input type="range" id="speed" min="0" max="0.1" step="0.001" value="0.01">
        <label>複素バランス (虚/実)</label>
        <input type="range" id="balance" min="0" max="2" step="0.1" value="1">
    </div>
</div>

<div id="status">Powered by Gemini - Quantum Geometry Logic</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
    let scene, camera, renderer, tetrahedron1, tetrahedron2, group;
    let step = 0;

    const steps = [
        {
            title: "Phase 1: 正四面体 (作用素の最小単位)",
            desc: "底面の3点は実数的な3次元空間。頂点の1点は虚数的な4次元。これこそが光を生み出すための最小の作用素です。",
            showSecond: false
        },
        {
            title: "Phase 2: マカバ (光の原構造)",
            desc: "反対向きの正四面体が重なり、マカバ（星型二重正四面体）となります。これでエネルギーの循環（光）が可能になります。",
            showSecond: true
        },
        {
            title: "Phase 3: スピン (アップとダウン)",
            desc: "マカバの回転は、物質粒子のアップスピンとダウンスピンを意味します。720度回転で元に戻る幾何学の神秘です。",
            showSecond: true
        }
    ];

    init();
    animate();

    function init() {
        scene = new THREE.Scene();
        camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
        camera.position.z = 5;

        renderer = new THREE.WebGLRenderer({ antialias: true });
        renderer.setSize(window.innerWidth, window.innerHeight);
        document.body.appendChild(renderer.domElement);

        group = new THREE.Group();
        scene.add(group);

        // 正四面体 1
        const geo1 = new THREE.TetrahedronGeometry(1.5);
        const mat1 = new THREE.MeshPhongMaterial({ color: 0x00d4ff, wireframe: true, transparent: true, opacity: 0.8 });
        tetrahedron1 = new THREE.Mesh(geo1, mat1);
        group.add(tetrahedron1);

        // 正四面体 2 (逆向き)
        const geo2 = new THREE.TetrahedronGeometry(1.5);
        const mat2 = new THREE.MeshPhongMaterial({ color: 0xff0066, wireframe: true, transparent: true, opacity: 0 });
        tetrahedron2 = new THREE.Mesh(geo2, mat2);
        tetrahedron2.rotation.x = Math.PI; // 逆転
        group.add(tetrahedron2);

        // ライト
        const light = new THREE.PointLight(0xffffff, 1, 100);
        light.position.set(10, 10, 10);
        scene.add(light);
        scene.add(new THREE.AmbientLight(0x404040));
    }

    function nextStep() {
        step = (step + 1) % steps.length;
        const s = steps[step];
        document.getElementById('title').innerText = s.title;
        document.getElementById('description').innerText = s.desc;
        
        if (s.showSecond) {
            tetrahedron2.material.opacity = 0.8;
        } else {
            tetrahedron2.material.opacity = 0;
        }
    }

    function animate() {
        requestAnimationFrame(animate);
        
        const speed = parseFloat(document.getElementById('speed').value);
        const balance = parseFloat(document.getElementById('balance').value);
        
        group.rotation.y += speed;
        group.rotation.z += speed * 0.5;
        
        tetrahedron1.scale.set(balance, balance, balance);
        tetrahedron2.scale.set(1/balance, 1/balance, 1/balance);

        renderer.render(scene, camera);
    }

    window.addEventListener('resize', () => {
        camera.aspect = window.innerWidth / window.innerHeight;
        camera.updateProjectionMatrix();
        renderer.setSize(window.innerWidth, window.innerHeight);
    });
</script>
</body>
</html>
