<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Generator Prompt Sobat Kere</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #111827;
            color: #d1d5db;
        }
        .form-section {
            background-color: #1f2937;
            border: 1px solid #374151;
            border-radius: 12px;
            padding: 24px;
            margin-bottom: 24px;
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
        }
        .form-section-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: #f9fafb;
            margin-bottom: 16px;
            border-bottom: 2px solid #4b5563;
            padding-bottom: 8px;
        }
        .sub-section-title {
            font-size: 1.1rem;
            font-weight: 600;
            color: #e5e7eb;
            margin-bottom: 12px;
            margin-top: 20px;
            border-bottom: 1px solid #4b5563;
            padding-bottom: 6px;
        }
        label {
            display: block;
            font-weight: 500;
            margin-bottom: 8px;
            color: #9ca3af;
        }
        .input-field, .select-field, .textarea-field {
            width: 100%;
            background-color: #374151;
            border: 1px solid #4b5563;
            color: #d1d5db;
            border-radius: 8px;
            padding: 10px;
            margin-bottom: 4px; /* Reduced margin */
            transition: border-color 0.3s, box-shadow 0.3s;
        }
        .input-field:focus, .select-field:focus, .textarea-field:focus {
            outline: none;
            border-color: #3b82f6;
            box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.5);
        }
        .input-container {
            margin-bottom: 16px;
        }
        .btn {
            padding: 12px 24px;
            border-radius: 8px;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.2s;
            border: none;
        }
        .btn-primary {
            background-color: #3b82f6;
            color: white;
        }
        .btn-primary:hover {
            background-color: #2563eb;
            transform: translateY(-2px);
        }
        .btn-secondary {
            background-color: #4b5563;
            color: white;
        }
        .btn-secondary:hover {
            background-color: #6b7280;
        }
        #output-container {
            background-color: #1f2937;
            border: 1px solid #374151;
            border-radius: 12px;
            padding: 24px;
            margin-top: 24px;
        }
        #prompt-output {
            width: 100%;
            height: 300px;
            background-color: #111827;
            border: 1px solid #4b5563;
            color: #e5e7eb;
            border-radius: 8px;
            padding: 12px;
            resize: vertical;
        }
        .hidden {
            display: none;
        }
        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 16px;
        }
        .important-note {
            background-color: #25395c;
            border-left: 4px solid #3b82f6;
            padding: 16px;
            border-radius: 8px;
            margin-bottom: 20px;
            color: #bfdbfe;
        }
        .negative-section {
            background-color: #374151; 
            border-left: 4px solid #6b7280; 
        }
        .other-input {
            margin-top: 8px;
        }
    </style>
</head>
<body class="p-4 sm:p-6 md:p-10">

    <div class="max-w-7xl mx-auto">
        <header class="text-center mb-10">
            <h1 class="text-3xl sm:text-4xl font-bold text-white">Generator Prompt Sobat Kere</h1>
            <p class="text-gray-400 mt-2">Dibuat untuk para kreator konten.</p>
        </header>

        <main id="prompt-form">
            <!-- Bagian Info Dasar -->
            <section class="form-section">
                <h2 class="form-section-title">Informasi Dasar Video</h2>
                <div class="grid-container">
                    <div class="input-container">
                        <label for="video-type">Jenis Video</label>
                        <input type="text" id="video-type" class="input-field" placeholder="Contoh: Film Pendek, Drama, Komedi">
                    </div>
                    <div class="input-container">
                        <label for="video-name">Nama / Judul Video</label>
                        <input type="text" id="video-name" class="input-field" placeholder="Contoh: Sore di Tepi Sawah">
                    </div>
                </div>
            </section>

            <!-- Bagian Catatan Penting -->
            <div class="important-note">
                <p><strong class="text-white">PENTING:</strong> Pastikan suara karakter konsisten. Untuk dialog Bahasa Jawa, gunakan logat Jawa Timur yang natural dan jelas.</p>
            </div>

            <!-- Karakter 1 -->
            <section class="form-section" id="character1-section">
                <h2 class="form-section-title">Karakter 1</h2>
                <div class="input-container mb-6">
                    <label for="c1-full-preset">Pilih Preset Detail (Baru)</label>
                    <select id="c1-full-preset" class="select-field">
                        <!-- Opsi Preset Detail akan diisi oleh JS -->
                    </select>
                </div>
                <div class="input-container mb-6">
                    <label for="c1-preset">Pilih Preset Ringkas (Lama)</label>
                    <select id="c1-preset" class="select-field">
                        <!-- Opsi Preset akan diisi oleh JS -->
                    </select>
                    <input type="text" id="c1-preset-other" class="input-field other-input hidden" placeholder="Tuliskan preset Anda...">
                </div>
                <!-- Konten Form Karakter 1 -->
                <div class="grid-container">
                    <div class="input-container col-span-full"><label for="c1-name">Nama Karakter</label><input type="text" id="c1-name" class="input-field" placeholder="Contoh: Siti"></div>
                    <div class="input-container"><label for="c1-age">Usia</label><select id="c1-age" class="select-field"></select><input type="text" id="c1-age-other" class="input-field other-input hidden" placeholder="Tuliskan usia..."></div>
                    <div class="input-container"><label for="c1-gender">Jenis Kelamin</label><select id="c1-gender" class="select-field"><option value="">Pilih</option><option value="Perempuan">Perempuan</option><option value="Laki-Laki">Laki-Laki</option></select><input type="text" id="c1-gender-other" class="input-field other-input hidden" placeholder="Tuliskan jenis kelamin..."></div>
                    <div class="input-container"><label for="c1-etnis">Etnis</label><select id="c1-etnis" class="select-field"></select><input type="text" id="c1-etnis-other" class="input-field other-input hidden" placeholder="Tuliskan etnis..."></div>
                    <div class="input-container col-span-full"><label for="c1-body">Perawakan/Bentuk Tubuh</label><textarea id="c1-body" class="textarea-field" rows="4" placeholder="Contoh: Ramping dan proporsional"></textarea></div>
                    <div class="input-container"><label for="c1-skin">Warna Kulit</label><select id="c1-skin" class="select-field"></select><input type="text" id="c1-skin-other" class="input-field other-input hidden" placeholder="Tuliskan warna kulit..."></div>
                    <div class="input-container"><label for="c1-breasts">Ukuran (Payudara)</label><select id="c1-breasts" class="select-field"></select><input type="text" id="c1-breasts-other" class="input-field other-input hidden" placeholder="Tuliskan ukuran..."></div>
                    <div class="input-container col-span-full"><label for="c1-face">Wajah</label><textarea id="c1-face" class="textarea-field" rows="4" placeholder="Contoh: Oval, rahang halus"></textarea></div>
                    <div class="input-container"><label for="c1-hair">Rambut</label><select id="c1-hair" class="select-field"></select><input type="text" id="c1-hair-other" class="input-field other-input hidden" placeholder="Tuliskan gaya rambut..."></div>
                    <div class="input-container"><label for="c1-top">Pakaian Atas</label><select id="c1-top" class="select-field"></select><input type="text" id="c1-top-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian atas..."></div>
                    <div class="input-container"><label for="c1-bottom">Pakaian Bawah</label><select id="c1-bottom" class="select-field"></select><input type="text" id="c1-bottom-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian bawah..."></div>
                    <div class="input-container"><label for="c1-accessory">Aksesori</label><select id="c1-accessory" class="select-field"></select><input type="text" id="c1-accessory-other" class="input-field other-input hidden" placeholder="Tuliskan aksesori..."></div>
                    <div class="col-span-full"><h3 class="sub-section-title">🎤 Suara Karakter 1</h3></div>
                    <div class="input-container"><label for="c1-voice-type">Jenis Suara</label><select id="c1-voice-type" class="select-field"><option value="">Pilih</option><option value="Sopran (Wanita Tertinggi)">Sopran (Wanita Tertinggi)</option><option value="Mezzo-Sopran (Wanita Halus)">Mezzo-Sopran (Wanita Halus)</option><option value="Alto (Wanita Terendah)">Alto (Wanita Terendah)</option><option value="Tenor (Pria Tertinggi)">Tenor (Pria Tertinggi)</option><option value="Bariton (Pria Halus)">Bariton (Pria Halus)</option><option value="Bass (Pria Terendah)">Bass (Pria Terendah)</option><option value="Countertenor (Pria Jangkauan Wanita)">Countertenor (Pria Jangkauan Wanita)</option></select><input type="text" id="c1-voice-type-other" class="input-field other-input hidden" placeholder="Tuliskan jenis suara..."></div>
                    <div class="input-container"><label for="c1-speech">Cara Berbicara</label><select id="c1-speech" class="select-field"><option value="">Pilih</option><option value="Antusias">Antusias</option><option value="Pelan">Pelan</option><option value="Sedang">Sedang</option><option value="Cepat">Cepat</option></select><input type="text" id="c1-speech-other" class="input-field other-input hidden" placeholder="Tuliskan cara berbicara..."></div>
                    <div class="input-container col-span-full"><label for="c1-accent">Aksen/Logat</label><select id="c1-accent" class="select-field"></select><input type="text" id="c1-accent-other" class="input-field other-input hidden" placeholder="Tuliskan aksen/logat..."></div>
                    <div class="input-container col-span-full"><label for="c1-voice-desc">Deskripsi Suara</label><select id="c1-voice-desc" class="select-field"></select><input type="text" id="c1-voice-desc-other" class="input-field other-input hidden" placeholder="Tuliskan deskripsi suara..."></div>
                </div>
            </section>
            
            <button id="add-character-btn-2" class="btn btn-secondary w-full mb-6">+ Tambah Karakter 2</button>

            <!-- Karakter 2 -->
            <section class="form-section hidden" id="character2-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">Karakter 2</h2><button id="remove-character-btn-2" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                <div class="input-container mb-6">
                    <label for="c2-full-preset">Pilih Preset Detail (Baru)</label>
                    <select id="c2-full-preset" class="select-field"></select>
                </div>
                <div class="input-container mb-6"><label for="c2-preset">Pilih Preset Ringkas (Lama)</label><select id="c2-preset" class="select-field"></select><input type="text" id="c2-preset-other" class="input-field other-input hidden" placeholder="Tuliskan preset Anda..."></div>
                <div class="grid-container">
                    <div class="input-container col-span-full"><label for="c2-name">Nama Karakter</label><input type="text" id="c2-name" class="input-field" placeholder="Contoh: Budi"></div>
                    <div class="input-container"><label for="c2-age">Usia</label><select id="c2-age" class="select-field"></select><input type="text" id="c2-age-other" class="input-field other-input hidden" placeholder="Tuliskan usia..."></div>
                    <div class="input-container"><label for="c2-gender">Jenis Kelamin</label><select id="c2-gender" class="select-field"><option value="">Pilih</option><option value="Perempuan">Perempuan</option><option value="Laki-Laki">Laki-Laki</option></select><input type="text" id="c2-gender-other" class="input-field other-input hidden" placeholder="Tuliskan jenis kelamin..."></div>
                    <div class="input-container"><label for="c2-etnis">Etnis</label><select id="c2-etnis" class="select-field"></select><input type="text" id="c2-etnis-other" class="input-field other-input hidden" placeholder="Tuliskan etnis..."></div>
                    <div class="input-container col-span-full"><label for="c2-body">Perawakan/Bentuk Tubuh</label><textarea id="c2-body" class="textarea-field" rows="4"></textarea></div>
                    <div class="input-container"><label for="c2-skin">Warna Kulit</label><select id="c2-skin" class="select-field"></select><input type="text" id="c2-skin-other" class="input-field other-input hidden" placeholder="Tuliskan warna kulit..."></div>
                    <div class="input-container"><label for="c2-breasts">Ukuran (Payudara)</label><select id="c2-breasts" class="select-field"></select><input type="text" id="c2-breasts-other" class="input-field other-input hidden" placeholder="Tuliskan ukuran..."></div>
                    <div class="input-container col-span-full"><label for="c2-face">Wajah</label><textarea id="c2-face" class="textarea-field" rows="4"></textarea></div>
                    <div class="input-container"><label for="c2-hair">Rambut</label><select id="c2-hair" class="select-field"></select><input type="text" id="c2-hair-other" class="input-field other-input hidden" placeholder="Tuliskan gaya rambut..."></div>
                    <div class="input-container"><label for="c2-top">Pakaian Atas</label><select id="c2-top" class="select-field"></select><input type="text" id="c2-top-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian atas..."></div>
                    <div class="input-container"><label for="c2-bottom">Pakaian Bawah</label><select id="c2-bottom" class="select-field"></select><input type="text" id="c2-bottom-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian bawah..."></div>
                    <div class="input-container"><label for="c2-accessory">Aksesori</label><select id="c2-accessory" class="select-field"></select><input type="text" id="c2-accessory-other" class="input-field other-input hidden" placeholder="Tuliskan aksesori..."></div>
                    <div class="col-span-full"><h3 class="sub-section-title">🎤 Suara Karakter 2</h3></div>
                    <div class="input-container"><label for="c2-voice-type">Jenis Suara</label><select id="c2-voice-type" class="select-field"><option value="">Pilih</option><option value="Sopran (Wanita Tertinggi)">Sopran (Wanita Tertinggi)</option><option value="Mezzo-Sopran (Wanita Halus)">Mezzo-Sopran (Wanita Halus)</option><option value="Alto (Wanita Terendah)">Alto (Wanita Terendah)</option><option value="Tenor (Pria Tertinggi)">Tenor (Pria Tertinggi)</option><option value="Bariton (Pria Halus)">Bariton (Pria Halus)</option><option value="Bass (Pria Terendah)">Bass (Pria Terendah)</option><option value="Countertenor (Pria Jangkauan Wanita)">Countertenor (Pria Jangkauan Wanita)</option></select><input type="text" id="c2-voice-type-other" class="input-field other-input hidden" placeholder="Tuliskan jenis suara..."></div>
                    <div class="input-container"><label for="c2-speech">Cara Berbicara</label><select id="c2-speech" class="select-field"><option value="">Pilih</option><option value="Antusias">Antusias</option><option value="Pelan">Pelan</option><option value="Sedang">Sedang</option><option value="Cepat">Cepat</option></select><input type="text" id="c2-speech-other" class="input-field other-input hidden" placeholder="Tuliskan cara berbicara..."></div>
                    <div class="input-container col-span-full"><label for="c2-accent">Aksen/Logat</label><select id="c2-accent" class="select-field"></select><input type="text" id="c2-accent-other" class="input-field other-input hidden" placeholder="Tuliskan aksen/logat..."></div>
                    <div class="input-container col-span-full"><label for="c2-voice-desc">Deskripsi Suara</label><select id="c2-voice-desc" class="select-field"></select><input type="text" id="c2-voice-desc-other" class="input-field other-input hidden" placeholder="Tuliskan deskripsi suara..."></div>
                </div>
                <button id="add-character-btn-3" class="btn btn-secondary w-full mt-6">+ Tambah Karakter 3</button>
            </section>

            <!-- Karakter 3 -->
            <section class="form-section hidden" id="character3-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">Karakter 3</h2><button id="remove-character-btn-3" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                 <div class="input-container mb-6">
                    <label for="c3-full-preset">Pilih Preset Detail (Baru)</label>
                    <select id="c3-full-preset" class="select-field"></select>
                </div>
                <div class="input-container mb-6"><label for="c3-preset">Pilih Preset Ringkas (Lama)</label><select id="c3-preset" class="select-field"></select><input type="text" id="c3-preset-other" class="input-field other-input hidden" placeholder="Tuliskan preset Anda..."></div>
                <div class="grid-container">
                    <div class="input-container col-span-full"><label for="c3-name">Nama Karakter</label><input type="text" id="c3-name" class="input-field"></div>
                    <div class="input-container"><label for="c3-age">Usia</label><select id="c3-age" class="select-field"></select><input type="text" id="c3-age-other" class="input-field other-input hidden" placeholder="Tuliskan usia..."></div>
                    <div class="input-container"><label for="c3-gender">Jenis Kelamin</label><select id="c3-gender" class="select-field"><option value="">Pilih</option><option value="Perempuan">Perempuan</option><option value="Laki-Laki">Laki-Laki</option></select><input type="text" id="c3-gender-other" class="input-field other-input hidden" placeholder="Tuliskan jenis kelamin..."></div>
                    <div class="input-container"><label for="c3-etnis">Etnis</label><select id="c3-etnis" class="select-field"></select><input type="text" id="c3-etnis-other" class="input-field other-input hidden" placeholder="Tuliskan etnis..."></div>
                    <div class="input-container col-span-full"><label for="c3-body">Perawakan/Bentuk Tubuh</label><textarea id="c3-body" class="textarea-field" rows="4"></textarea></div>
                    <div class="input-container"><label for="c3-skin">Warna Kulit</label><select id="c3-skin" class="select-field"></select><input type="text" id="c3-skin-other" class="input-field other-input hidden" placeholder="Tuliskan warna kulit..."></div>
                    <div class="input-container"><label for="c3-breasts">Ukuran (Payudara)</label><select id="c3-breasts" class="select-field"></select><input type="text" id="c3-breasts-other" class="input-field other-input hidden" placeholder="Tuliskan ukuran..."></div>
                    <div class="input-container col-span-full"><label for="c3-face">Wajah</label><textarea id="c3-face" class="textarea-field" rows="4"></textarea></div>
                    <div class="input-container"><label for="c3-hair">Rambut</label><select id="c3-hair" class="select-field"></select><input type="text" id="c3-hair-other" class="input-field other-input hidden" placeholder="Tuliskan gaya rambut..."></div>
                    <div class="input-container"><label for="c3-top">Pakaian Atas</label><select id="c3-top" class="select-field"></select><input type="text" id="c3-top-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian atas..."></div>
                    <div class="input-container"><label for="c3-bottom">Pakaian Bawah</label><select id="c3-bottom" class="select-field"></select><input type="text" id="c3-bottom-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian bawah..."></div>
                    <div class="input-container"><label for="c3-accessory">Aksesori</label><select id="c3-accessory" class="select-field"></select><input type="text" id="c3-accessory-other" class="input-field other-input hidden" placeholder="Tuliskan aksesori..."></div>
                    <div class="col-span-full"><h3 class="sub-section-title">🎤 Suara Karakter 3</h3></div>
                    <div class="input-container"><label for="c3-voice-type">Jenis Suara</label><select id="c3-voice-type" class="select-field"><option value="">Pilih</option><option value="Sopran (Wanita Tertinggi)">Sopran (Wanita Tertinggi)</option><option value="Mezzo-Sopran (Wanita Halus)">Mezzo-Sopran (Wanita Halus)</option><option value="Alto (Wanita Terendah)">Alto (Wanita Terendah)</option><option value="Tenor (Pria Tertinggi)">Tenor (Pria Tertinggi)</option><option value="Bariton (Pria Halus)">Bariton (Pria Halus)</option><option value="Bass (Pria Terendah)">Bass (Pria Terendah)</option><option value="Countertenor (Pria Jangkauan Wanita)">Countertenor (Pria Jangkauan Wanita)</option></select><input type="text" id="c3-voice-type-other" class="input-field other-input hidden" placeholder="Tuliskan jenis suara..."></div>
                    <div class="input-container"><label for="c3-speech">Cara Berbicara</label><select id="c3-speech" class="select-field"><option value="">Pilih</option><option value="Antusias">Antusias</option><option value="Pelan">Pelan</option><option value="Sedang">Sedang</option><option value="Cepat">Cepat</option></select><input type="text" id="c3-speech-other" class="input-field other-input hidden" placeholder="Tuliskan cara berbicara..."></div>
                    <div class="input-container col-span-full"><label for="c3-accent">Aksen/Logat</label><select id="c3-accent" class="select-field"></select><input type="text" id="c3-accent-other" class="input-field other-input hidden" placeholder="Tuliskan aksen/logat..."></div>
                    <div class="input-container col-span-full"><label for="c3-voice-desc">Deskripsi Suara</label><select id="c3-voice-desc" class="select-field"></select><input type="text" id="c3-voice-desc-other" class="input-field other-input hidden" placeholder="Tuliskan deskripsi suara..."></div>
                </div>
                <button id="add-character-btn-4" class="btn btn-secondary w-full mt-6">+ Tambah Karakter 4</button>
            </section>

            <!-- Karakter 4 -->
            <section class="form-section hidden" id="character4-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">Karakter 4</h2><button id="remove-character-btn-4" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                <div class="input-container mb-6">
                    <label for="c4-full-preset">Pilih Preset Detail (Baru)</label>
                    <select id="c4-full-preset" class="select-field"></select>
                </div>
                <div class="input-container mb-6"><label for="c4-preset">Pilih Preset Ringkas (Lama)</label><select id="c4-preset" class="select-field"></select><input type="text" id="c4-preset-other" class="input-field other-input hidden" placeholder="Tuliskan preset Anda..."></div>
                <div class="grid-container">
                     <div class="input-container col-span-full"><label for="c4-name">Nama Karakter</label><input type="text" id="c4-name" class="input-field"></div>
                    <div class="input-container"><label for="c4-age">Usia</label><select id="c4-age" class="select-field"></select><input type="text" id="c4-age-other" class="input-field other-input hidden" placeholder="Tuliskan usia..."></div>
                    <div class="input-container"><label for="c4-gender">Jenis Kelamin</label><select id="c4-gender" class="select-field"><option value="">Pilih</option><option value="Perempuan">Perempuan</option><option value="Laki-Laki">Laki-Laki</option></select><input type="text" id="c4-gender-other" class="input-field other-input hidden" placeholder="Tuliskan jenis kelamin..."></div>
                    <div class="input-container"><label for="c4-etnis">Etnis</label><select id="c4-etnis" class="select-field"></select><input type="text" id="c4-etnis-other" class="input-field other-input hidden" placeholder="Tuliskan etnis..."></div>
                    <div class="input-container col-span-full"><label for="c4-body">Perawakan/Bentuk Tubuh</label><textarea id="c4-body" class="textarea-field" rows="4"></textarea></div>
                    <div class="input-container"><label for="c4-skin">Warna Kulit</label><select id="c4-skin" class="select-field"></select><input type="text" id="c4-skin-other" class="input-field other-input hidden" placeholder="Tuliskan warna kulit..."></div>
                    <div class="input-container"><label for="c4-breasts">Ukuran (Payudara)</label><select id="c4-breasts" class="select-field"></select><input type="text" id="c4-breasts-other" class="input-field other-input hidden" placeholder="Tuliskan ukuran..."></div>
                    <div class="input-container col-span-full"><label for="c4-face">Wajah</label><textarea id="c4-face" class="textarea-field" rows="4"></textarea></div>
                    <div class="input-container"><label for="c4-hair">Rambut</label><select id="c4-hair" class="select-field"></select><input type="text" id="c4-hair-other" class="input-field other-input hidden" placeholder="Tuliskan gaya rambut..."></div>
                    <div class="input-container"><label for="c4-top">Pakaian Atas</label><select id="c4-top" class="select-field"></select><input type="text" id="c4-top-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian atas..."></div>
                    <div class="input-container"><label for="c4-bottom">Pakaian Bawah</label><select id="c4-bottom" class="select-field"></select><input type="text" id="c4-bottom-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian bawah..."></div>
                    <div class="input-container"><label for="c4-accessory">Aksesori</label><select id="c4-accessory" class="select-field"></select><input type="text" id="c4-accessory-other" class="input-field other-input hidden" placeholder="Tuliskan aksesori..."></div>
                    <div class="col-span-full"><h3 class="sub-section-title">🎤 Suara Karakter 4</h3></div>
                    <div class="input-container"><label for="c4-voice-type">Jenis Suara</label><select id="c4-voice-type" class="select-field"><option value="">Pilih</option><option value="Sopran (Wanita Tertinggi)">Sopran (Wanita Tertinggi)</option><option value="Mezzo-Sopran (Wanita Halus)">Mezzo-Sopran (Wanita Halus)</option><option value="Alto (Wanita Terendah)">Alto (Wanita Terendah)</option><option value="Tenor (Pria Tertinggi)">Tenor (Pria Tertinggi)</option><option value="Bariton (Pria Halus)">Bariton (Pria Halus)</option><option value="Bass (Pria Terendah)">Bass (Pria Terendah)</option><option value="Countertenor (Pria Jangkauan Wanita)">Countertenor (Pria Jangkauan Wanita)</option></select><input type="text" id="c4-voice-type-other" class="input-field other-input hidden" placeholder="Tuliskan jenis suara..."></div>
                    <div class="input-container"><label for="c4-speech">Cara Berbicara</label><select id="c4-speech" class="select-field"><option value="">Pilih</option><option value="Antusias">Antusias</option><option value="Pelan">Pelan</option><option value="Sedang">Sedang</option><option value="Cepat">Cepat</option></select><input type="text" id="c4-speech-other" class="input-field other-input hidden" placeholder="Tuliskan cara berbicara..."></div>
                    <div class="input-container col-span-full"><label for="c4-accent">Aksen/Logat</label><select id="c4-accent" class="select-field"></select><input type="text" id="c4-accent-other" class="input-field other-input hidden" placeholder="Tuliskan aksen/logat..."></div>
                    <div class="input-container col-span-full"><label for="c4-voice-desc">Deskripsi Suara</label><select id="c4-voice-desc" class="select-field"></select><input type="text" id="c4-voice-desc-other" class="input-field other-input hidden" placeholder="Tuliskan deskripsi suara..."></div>
                </div>
                 <button id="add-character-btn-5" class="btn btn-secondary w-full mt-6">+ Tambah Karakter 5</button>
            </section>
            
            <!-- Karakter 5 -->
            <section class="form-section hidden" id="character5-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">Karakter 5</h2><button id="remove-character-btn-5" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                <div class="input-container mb-6">
                    <label for="c5-full-preset">Pilih Preset Detail (Baru)</label>
                    <select id="c5-full-preset" class="select-field"></select>
                </div>
                <div class="input-container mb-6"><label for="c5-preset">Pilih Preset Ringkas (Lama)</label><select id="c5-preset" class="select-field"></select><input type="text" id="c5-preset-other" class="input-field other-input hidden" placeholder="Tuliskan preset Anda..."></div>
                <div class="grid-container">
                    <div class="input-container col-span-full"><label for="c5-name">Nama Karakter</label><input type="text" id="c5-name" class="input-field"></div>
                    <div class="input-container"><label for="c5-age">Usia</label><select id="c5-age" class="select-field"></select><input type="text" id="c5-age-other" class="input-field other-input hidden" placeholder="Tuliskan usia..."></div>
                    <div class="input-container"><label for="c5-gender">Jenis Kelamin</label><select id="c5-gender" class="select-field"><option value="">Pilih</option><option value="Perempuan">Perempuan</option><option value="Laki-Laki">Laki-Laki</option></select><input type="text" id="c5-gender-other" class="input-field other-input hidden" placeholder="Tuliskan jenis kelamin..."></div>
                    <div class="input-container"><label for="c5-etnis">Etnis</label><select id="c5-etnis" class="select-field"></select><input type="text" id="c5-etnis-other" class="input-field other-input hidden" placeholder="Tuliskan etnis..."></div>
                    <div class="input-container col-span-full"><label for="c5-body">Perawakan/Bentuk Tubuh</label><textarea id="c5-body" class="textarea-field" rows="4"></textarea></div>
                    <div class="input-container"><label for="c5-skin">Warna Kulit</label><select id="c5-skin" class="select-field"></select><input type="text" id="c5-skin-other" class="input-field other-input hidden" placeholder="Tuliskan warna kulit..."></div>
                    <div class="input-container"><label for="c5-breasts">Ukuran (Payudara)</label><select id="c5-breasts" class="select-field"></select><input type="text" id="c5-breasts-other" class="input-field other-input hidden" placeholder="Tuliskan ukuran..."></div>
                    <div class="input-container col-span-full"><label for="c5-face">Wajah</label><textarea id="c5-face" class="textarea-field" rows="4"></textarea></div>
                    <div class="input-container"><label for="c5-hair">Rambut</label><select id="c5-hair" class="select-field"></select><input type="text" id="c5-hair-other" class="input-field other-input hidden" placeholder="Tuliskan gaya rambut..."></div>
                    <div class="input-container"><label for="c5-top">Pakaian Atas</label><select id="c5-top" class="select-field"></select><input type="text" id="c5-top-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian atas..."></div>
                    <div class="input-container"><label for="c5-bottom">Pakaian Bawah</label><select id="c5-bottom" class="select-field"></select><input type="text" id="c5-bottom-other" class="input-field other-input hidden" placeholder="Tuliskan pakaian bawah..."></div>
                    <div class="input-container"><label for="c5-accessory">Aksesori</label><select id="c5-accessory" class="select-field"></select><input type="text" id="c5-accessory-other" class="input-field other-input hidden" placeholder="Tuliskan aksesori..."></div>
                    <div class="col-span-full"><h3 class="sub-section-title">🎤 Suara Karakter 5</h3></div>
                    <div class="input-container"><label for="c5-voice-type">Jenis Suara</label><select id="c5-voice-type" class="select-field"><option value="">Pilih</option><option value="Sopran (Wanita Tertinggi)">Sopran (Wanita Tertinggi)</option><option value="Mezzo-Sopran (Wanita Halus)">Mezzo-Sopran (Wanita Halus)</option><option value="Alto (Wanita Terendah)">Alto (Wanita Terendah)</option><option value="Tenor (Pria Tertinggi)">Tenor (Pria Tertinggi)</option><option value="Bariton (Pria Halus)">Bariton (Pria Halus)</option><option value="Bass (Pria Terendah)">Bass (Pria Terendah)</option><option value="Countertenor (Pria Jangkauan Wanita)">Countertenor (Pria Jangkauan Wanita)</option></select><input type="text" id="c5-voice-type-other" class="input-field other-input hidden" placeholder="Tuliskan jenis suara..."></div>
                    <div class="input-container"><label for="c5-speech">Cara Berbicara</label><select id="c5-speech" class="select-field"><option value="">Pilih</option><option value="Antusias">Antusias</option><option value="Pelan">Pelan</option><option value="Sedang">Sedang</option><option value="Cepat">Cepat</option></select><input type="text" id="c5-speech-other" class="input-field other-input hidden" placeholder="Tuliskan cara berbicara..."></div>
                    <div class="input-container col-span-full"><label for="c5-accent">Aksen/Logat</label><select id="c5-accent" class="select-field"></select><input type="text" id="c5-accent-other" class="input-field other-input hidden" placeholder="Tuliskan aksen/logat..."></div>
                    <div class="input-container col-span-full"><label for="c5-voice-desc">Deskripsi Suara</label><select id="c5-voice-desc" class="select-field"></select><input type="text" id="c5-voice-desc-other" class="input-field other-input hidden" placeholder="Tuliskan deskripsi suara..."></div>
                </div>
            </section>
            
            <!-- Scene 1 -->
            <section class="form-section" id="scene1-section">
                <h2 class="form-section-title">🎬 Scene 1</h2>
                <div class="grid-container">
                    <div class="col-span-full"><h3 class="sub-section-title">🎭 Detail Adegan</h3></div>
                    <div class="input-container col-span-full"><label for="s1-characters">Karakter Terlibat</label><input type="text" id="s1-characters" class="input-field" placeholder="Contoh: Siti, Budi"></div>
                    <div class="input-container col-span-full"><label for="s1-action">Aksi Karakter</label><textarea id="s1-action" class="textarea-field" rows="2" placeholder="Contoh: Siti berjalan perlahan, Budi menuangkan teh"></textarea></div>
                    <div class="input-container col-span-full"><label for="s1-expression">Ekspresi Karakter</label><textarea id="s1-expression" class="textarea-field" rows="2" placeholder="Contoh: Wajah Siti cemas, Budi tersenyum tipis"></textarea></div>
                    
                    <div class="col-span-full"><h3 class="sub-section-title">💬 Dialog</h3></div>
                    <div class="input-container col-span-full"><label for="s1-dialog-lang">Bahasa Dialog</label><select id="s1-dialog-lang" class="select-field"><option value="">Pilih</option><option value="Bahasa Jawa">Bahasa Jawa</option><option value="Bahasa Indonesia">Bahasa Indonesia</option><option value="Bahasa Sunda">Bahasa Sunda</option><option value="Bahasa Madura">Bahasa Madura</option><option value="Bahasa Minang">Bahasa Minang</option><option value="Bahasa Aceh">Bahasa Aceh</option><option value="Bahasa Dayak">Bahasa Dayak</option><option value="Bahasa Inggris">Bahasa Inggris</option><option value="Bahasa Jepang">Bahasa Jepang</option><option value="Bahasa Korea">Bahasa Korea</option></select><input type="text" id="s1-dialog-lang-other" class="input-field other-input hidden" placeholder="Tuliskan bahasa..."></div>
                    <div class="input-container col-span-full"><label for="s1-dialog">Teks Dialog</label><textarea id="s1-dialog" class="textarea-field" rows="6" placeholder="Masukkan dialog untuk scene ini..."></textarea></div>
                </div>
            </section>

            <button id="add-scene-btn-2" class="btn btn-secondary w-full mb-6">+ Tambah Scene 2</button>

            <!-- Scene 2 -->
            <section class="form-section hidden" id="scene2-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">🎬 Scene 2</h2><button id="remove-scene-btn-2" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                <div class="grid-container">
                    <div class="col-span-full"><h3 class="sub-section-title">🎭 Detail Adegan</h3></div>
                    <div class="input-container col-span-full"><label for="s2-characters">Karakter Terlibat</label><input type="text" id="s2-characters" class="input-field" placeholder="Contoh: Siti, Budi"></div>
                    <div class="input-container col-span-full"><label for="s2-action">Aksi Karakter</label><textarea id="s2-action" class="textarea-field" rows="2"></textarea></div>
                    <div class="input-container col-span-full"><label for="s2-expression">Ekspresi Karakter</label><textarea id="s2-expression" class="textarea-field" rows="2"></textarea></div>

                    <div class="col-span-full"><h3 class="sub-section-title">💬 Dialog</h3></div>
                    <div class="input-container col-span-full"><label for="s2-dialog-lang">Bahasa Dialog</label><select id="s2-dialog-lang" class="select-field"><option value="">Pilih</option><option value="Bahasa Jawa">Bahasa Jawa</option><option value="Bahasa Indonesia">Bahasa Indonesia</option><option value="Bahasa Sunda">Bahasa Sunda</option><option value="Bahasa Madura">Bahasa Madura</option><option value="Bahasa Minang">Bahasa Minang</option><option value="Bahasa Aceh">Bahasa Aceh</option><option value="Bahasa Dayak">Bahasa Dayak</option><option value="Bahasa Inggris">Bahasa Inggris</option><option value="Bahasa Jepang">Bahasa Jepang</option><option value="Bahasa Korea">Bahasa Korea</option></select><input type="text" id="s2-dialog-lang-other" class="input-field other-input hidden" placeholder="Tuliskan bahasa..."></div>
                    <div class="input-container col-span-full"><label for="s2-dialog">Teks Dialog</label><textarea id="s2-dialog" class="textarea-field" rows="6" placeholder="Masukkan dialog untuk scene ini..."></textarea></div>
                </div>
            </section>
            
            <button id="add-scene-btn-3" class="btn btn-secondary w-full mb-6 hidden">+ Tambah Scene 3</button>

            <!-- Scene 3 -->
            <section class="form-section hidden" id="scene3-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">🎬 Scene 3</h2><button id="remove-scene-btn-3" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                <div class="grid-container">
                    <div class="col-span-full"><h3 class="sub-section-title">🎭 Detail Adegan</h3></div>
                    <div class="input-container col-span-full"><label for="s3-characters">Karakter Terlibat</label><input type="text" id="s3-characters" class="input-field" placeholder="Contoh: Siti, Budi"></div>
                    <div class="input-container col-span-full"><label for="s3-action">Aksi Karakter</label><textarea id="s3-action" class="textarea-field" rows="2"></textarea></div>
                    <div class="input-container col-span-full"><label for="s3-expression">Ekspresi Karakter</label><textarea id="s3-expression" class="textarea-field" rows="2"></textarea></div>

                    <div class="col-span-full"><h3 class="sub-section-title">💬 Dialog</h3></div>
                    <div class="input-container col-span-full"><label for="s3-dialog-lang">Bahasa Dialog</label><select id="s3-dialog-lang" class="select-field"><option value="">Pilih</option><option value="Bahasa Jawa">Bahasa Jawa</option><option value="Bahasa Indonesia">Bahasa Indonesia</option><option value="Bahasa Sunda">Bahasa Sunda</option><option value="Bahasa Madura">Bahasa Madura</option><option value="Bahasa Minang">Bahasa Minang</option><option value="Bahasa Aceh">Bahasa Aceh</option><option value="Bahasa Dayak">Bahasa Dayak</option><option value="Bahasa Inggris">Bahasa Inggris</option><option value="Bahasa Jepang">Bahasa Jepang</option><option value="Bahasa Korea">Bahasa Korea</option></select><input type="text" id="s3-dialog-lang-other" class="input-field other-input hidden" placeholder="Tuliskan bahasa..."></div>
                    <div class="input-container col-span-full"><label for="s3-dialog">Teks Dialog</label><textarea id="s3-dialog" class="textarea-field" rows="6" placeholder="Masukkan dialog untuk scene ini..."></textarea></div>
                </div>
            </section>

            <button id="add-scene-btn-4" class="btn btn-secondary w-full mb-6 hidden">+ Tambah Scene 4</button>

            <!-- Scene 4 -->
            <section class="form-section hidden" id="scene4-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">🎬 Scene 4</h2><button id="remove-scene-btn-4" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                <div class="grid-container">
                    <div class="col-span-full"><h3 class="sub-section-title">🎭 Detail Adegan</h3></div>
                    <div class="input-container col-span-full"><label for="s4-characters">Karakter Terlibat</label><input type="text" id="s4-characters" class="input-field" placeholder="Contoh: Siti, Budi"></div>
                    <div class="input-container col-span-full"><label for="s4-action">Aksi Karakter</label><textarea id="s4-action" class="textarea-field" rows="2"></textarea></div>
                    <div class="input-container col-span-full"><label for="s4-expression">Ekspresi Karakter</label><textarea id="s4-expression" class="textarea-field" rows="2"></textarea></div>

                    <div class="col-span-full"><h3 class="sub-section-title">💬 Dialog</h3></div>
                    <div class="input-container col-span-full"><label for="s4-dialog-lang">Bahasa Dialog</label><select id="s4-dialog-lang" class="select-field"><option value="">Pilih</option><option value="Bahasa Jawa">Bahasa Jawa</option><option value="Bahasa Indonesia">Bahasa Indonesia</option><option value="Bahasa Sunda">Bahasa Sunda</option><option value="Bahasa Madura">Bahasa Madura</option><option value="Bahasa Minang">Bahasa Minang</option><option value="Bahasa Aceh">Bahasa Aceh</option><option value="Bahasa Dayak">Bahasa Dayak</option><option value="Bahasa Inggris">Bahasa Inggris</option><option value="Bahasa Jepang">Bahasa Jepang</option><option value="Bahasa Korea">Bahasa Korea</option></select><input type="text" id="s4-dialog-lang-other" class="input-field other-input hidden" placeholder="Tuliskan bahasa..."></div>
                    <div class="input-container col-span-full"><label for="s4-dialog">Teks Dialog</label><textarea id="s4-dialog" class="textarea-field" rows="6" placeholder="Masukkan dialog untuk scene ini..."></textarea></div>
                </div>
            </section>

            <button id="add-scene-btn-5" class="btn btn-secondary w-full mb-6 hidden">+ Tambah Scene 5</button>

            <!-- Scene 5 -->
            <section class="form-section hidden" id="scene5-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">🎬 Scene 5</h2><button id="remove-scene-btn-5" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                <div class="grid-container">
                    <div class="col-span-full"><h3 class="sub-section-title">🎭 Detail Adegan</h3></div>
                    <div class="input-container col-span-full"><label for="s5-characters">Karakter Terlibat</label><input type="text" id="s5-characters" class="input-field" placeholder="Contoh: Siti, Budi"></div>
                    <div class="input-container col-span-full"><label for="s5-action">Aksi Karakter</label><textarea id="s5-action" class="textarea-field" rows="2"></textarea></div>
                    <div class="input-container col-span-full"><label for="s5-expression">Ekspresi Karakter</label><textarea id="s5-expression" class="textarea-field" rows="2"></textarea></div>

                    <div class="col-span-full"><h3 class="sub-section-title">💬 Dialog</h3></div>
                    <div class="input-container col-span-full"><label for="s5-dialog-lang">Bahasa Dialog</label><select id="s5-dialog-lang" class="select-field"><option value="">Pilih</option><option value="Bahasa Jawa">Bahasa Jawa</option><option value="Bahasa Indonesia">Bahasa Indonesia</option><option value="Bahasa Sunda">Bahasa Sunda</option><option value="Bahasa Madura">Bahasa Madura</option><option value="Bahasa Minang">Bahasa Minang</option><option value="Bahasa Aceh">Bahasa Aceh</option><option value="Bahasa Dayak">Bahasa Dayak</option><option value="Bahasa Inggris">Bahasa Inggris</option><option value="Bahasa Jepang">Bahasa Jepang</option><option value="Bahasa Korea">Bahasa Korea</option></select><input type="text" id="s5-dialog-lang-other" class="input-field other-input hidden" placeholder="Tuliskan bahasa..."></div>
                    <div class="input-container col-span-full"><label for="s5-dialog">Teks Dialog</label><textarea id="s5-dialog" class="textarea-field" rows="6" placeholder="Masukkan dialog untuk scene ini..."></textarea></div>
                </div>
            </section>

            <button id="add-scene-btn-6" class="btn btn-secondary w-full mb-6 hidden">+ Tambah Scene 6</button>

            <!-- Scene 6 -->
            <section class="form-section hidden" id="scene6-section">
                <div class="flex justify-between items-center"><h2 class="form-section-title">🎬 Scene 6</h2><button id="remove-scene-btn-6" class="text-red-400 hover:text-red-600 font-bold">Hapus</button></div>
                <div class="grid-container">
                    <div class="col-span-full"><h3 class="sub-section-title">🎭 Detail Adegan</h3></div>
                    <div class="input-container col-span-full"><label for="s6-characters">Karakter Terlibat</label><input type="text" id="s6-characters" class="input-field" placeholder="Contoh: Siti, Budi"></div>
                    <div class="input-container col-span-full"><label for="s6-action">Aksi Karakter</label><textarea id="s6-action" class="textarea-field" rows="2"></textarea></div>
                    <div class="input-container col-span-full"><label for="s6-expression">Ekspresi Karakter</label><textarea id="s6-expression" class="textarea-field" rows="2"></textarea></div>

                    <div class="col-span-full"><h3 class="sub-section-title">💬 Dialog</h3></div>
                    <div class="input-container col-span-full"><label for="s6-dialog-lang">Bahasa Dialog</label><select id="s6-dialog-lang" class="select-field"><option value="">Pilih</option><option value="Bahasa Jawa">Bahasa Jawa</option><option value="Bahasa Indonesia">Bahasa Indonesia</option><option value="Bahasa Sunda">Bahasa Sunda</option><option value="Bahasa Madura">Bahasa Madura</option><option value="Bahasa Minang">Bahasa Minang</option><option value="Bahasa Aceh">Bahasa Aceh</option><option value="Bahasa Dayak">Bahasa Dayak</option><option value="Bahasa Inggris">Bahasa Inggris</option><option value="Bahasa Jepang">Bahasa Jepang</option><option value="Bahasa Korea">Bahasa Korea</option></select><input type="text" id="s6-dialog-lang-other" class="input-field other-input hidden" placeholder="Tuliskan bahasa..."></div>
                    <div class="input-container col-span-full"><label for="s6-dialog">Teks Dialog</label><textarea id="s6-dialog" class="textarea-field" rows="6" placeholder="Masukkan dialog untuk scene ini..."></textarea></div>
                </div>
            </section>

            <!-- Latar Tempat & Waktu Global -->
            <section class="form-section">
                <h2 class="form-section-title">🌍 Latar Tempat & Waktu (Global)</h2>
                <div class="grid-container">
                    <div class="input-container"><label for="global-village">Desa</label><input type="text" id="global-village" class="input-field" placeholder="Contoh: Kertajaya"></div>
                    <div class="input-container"><label for="global-setting">Latar Tempat</label><input type="text" id="global-setting" class="input-field" placeholder="Contoh: Teras belakang rumah"></div>
                    <div class="input-container">
                        <label for="global-weather">Cuaca</label>
                        <select id="global-weather" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Cerah">Cerah</option>
                            <option value="Berawan">Berawan</option>
                            <option value="Mendung">Mendung</option>
                            <option value="Hujan Ringan">Hujan Ringan</option>
                            <option value="Hujan Deras">Hujan Deras</option>
                            <option value="Badai Petir">Badai Petir</option>
                            <option value="Berkabut">Berkabut</option>
                        </select>
                        <input type="text" id="global-weather-other" class="input-field other-input hidden" placeholder="Tuliskan cuaca...">
                    </div>
                    <div class="input-container">
                        <label for="global-season">Musim</label>
                        <select id="global-season" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Musim Kemarau">Musim Kemarau</option>
                            <option value="Musim Hujan">Musim Hujan</option>
                            <option value="Musim Semi">Musim Semi</option>
                            <option value="Musim Gugur">Musim Gugur</option>
                            <option value="Musim Dingin">Musim Dingin</option>
                        </select>
                        <input type="text" id="global-season-other" class="input-field other-input hidden" placeholder="Tuliskan musim...">
                    </div>
                    <div class="input-container">
                        <label for="global-time">Waktu</label>
                        <select id="global-time" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Pagi">Pagi</option>
                            <option value="Siang">Siang</option>
                            <option value="Sore">Sore</option>
                            <option value="Malam">Malam</option>
                        </select>
                         <input type="text" id="global-time-other" class="input-field other-input hidden" placeholder="Tuliskan waktu...">
                    </div>
                    <div class="input-container">
                        <label for="global-clock">Jam</label>
                        <input type="text" id="global-clock" class="input-field" placeholder="Contoh: 16:30">
                    </div>
                </div>
            </section>

            <!-- Bagian Teknis & Visual Global -->
            <section class="form-section">
                <h2 class="form-section-title">Detail Teknis & Visual (Global)</h2>
                <div class="grid-container">
                    <div class="input-container">
                        <label for="overall-mood">Suasana Keseluruhan</label>
                        <select id="overall-mood" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Damai dan Tenang">Damai dan Tenang</option>
                            <option value="Melankolis">Melankolis</option>
                            <option value="Penuh Harapan">Penuh Harapan</option>
                            <option value="Misterius">Misterius</option>
                            <option value="Dramatis">Dramatis</option>
                            <option value="Suram">Suram</option>
                            <option value="Romantis">Romantis</option>
                        </select>
                        <input type="text" id="overall-mood-other" class="input-field other-input hidden" placeholder="Tuliskan suasana...">
                    </div>
                    <div class="input-container"><label for="ambience">Suara Lingkungan / Ambiance</label><input type="text" id="ambience" class="input-field" placeholder="Contoh: Rintik hujan, jangkrik"></div>
                    <div class="input-container">
                        <label for="art-style">🎨 Gaya Visual</label>
                        <select id="art-style" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Realistic">Realistic</option>
                            <option value="Cinematic Realistic">Cinematic Realistic</option>
                            <option value="Film Noir">Film Noir</option>
                            <option value="3D Animation">3D Animation</option>
                            <option value="Lukisan Cat Air Bergerak">Lukisan Cat Air Bergerak</option>
                            <option value="Dokumenter">Dokumenter</option>
                            <option value="Sci-Fi">Sci-Fi</option>
                            <option value="Fantasi">Fantasi</option>
                            <option value="Vintage">Vintage</option>
                            <option value="Anime">Anime</option>
                            <option value="Kartun">Kartun</option>
                        </select>
                        <input type="text" id="art-style-other" class="input-field other-input hidden" placeholder="Tuliskan gaya visual...">
                    </div>
                    <div class="input-container">
                        <label for="quality">Kualitas Visual</label>
                        <select id="quality" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Resolusi 8K">8K</option>
                            <option value="Resolusi 4K">4K</option>
                            <option value="Full HD">Full HD</option>
                            <option value="HD+">HD+</option>
                        </select>
                        <input type="text" id="quality-other" class="input-field other-input hidden" placeholder="Tuliskan kualitas...">
                    </div>
                    <div class="input-container">
                        <label for="lighting">💡 Pencahayaan</label>
                        <select id="lighting" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Cahaya Matahari Pagi">Cahaya Matahari Pagi</option>
                            <option value="Cahaya Senja Keemasan">Cahaya Senja Keemasan</option>
                            <option value="Cahaya Malam Kota">Cahaya Malam Kota</option>
                            <option value="Pencahayaan Remang-remang">Pencahayaan Remang-remang</option>
                            <option value="Pencahayaan Terang">Pencahayaan Terang</option>
                            <option value="Cahaya Dramatis">Cahaya Dramatis</option>
                            <option value="Cahaya Neon">Cahaya Neon</option>
                            <option value="Cahaya Ethereal/Magis">Cahaya Ethereal/Magis</option>
                        </select>
                        <input type="text" id="lighting-other" class="input-field other-input hidden" placeholder="Tuliskan pencahayaan...">
                    </div>
                    <div class="input-container">
                        <label for="camera-angle">🎥 Sudut Kamera</label>
                        <select id="camera-angle" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Medium Shot">Medium Shot</option>
                            <option value="Close-up">Close-up</option>
                            <option value="Wide Shot">Wide Shot</option>
                            <option value="Eye-level Shot">Eye-level Shot</option>
                            <option value="Low-angle Shot">Low-angle Shot</option>
                            <option value="High-angle Shot">High-angle Shot</option>
                            <option value="Over-the-Shoulder Shot">Over-the-Shoulder Shot</option>
                        </select>
                        <input type="text" id="camera-angle-other" class="input-field other-input hidden" placeholder="Tuliskan sudut kamera...">
                    </div>
                    <div class="input-container col-span-full">
                        <label for="camera-movement">Gerakan Kamera</label>
                        <select id="camera-movement" class="select-field">
                            <option value="">Pilih</option>
                            <option value="Static Shot (Kamera Diam)">Static Shot (Kamera Diam)</option>
                            <option value="Pan (Kiri/Kanan)">Pan (Kiri/Kanan)</option>
                            <option value="Tilt (Atas/Bawah)">Tilt (Atas/Bawah)</option>
                            <option value="Dolly (Maju/Mundur)">Dolly (Maju/Mundur)</option>
                            <option value="Truck (Geser Kiri/Kanan)">Truck (Geser Kiri/Kanan)</option>
                            <option value="Zoom (Perbesar/Perkecil)">Zoom (Perbesar/Perkecil)</option>
                            <option value="Tracking/Follow Shot (Mengikuti Objek)">Tracking/Follow Shot (Mengikuti Objek)</option>
                            <option value="Crane/Jib Shot (Gerakan Vertikal)">Crane/Jib Shot (Gerakan Vertikal)</option>
                            <option value="Handheld (Genggam)">Handheld (Genggam)</option>
                            <option value="Rotate (Putar Searah Jarum Jam)">Rotate (Putar Searah Jarum Jam)</option>
                            <option value="Rotate (Putar Berlawanan Jarum Jam)">Rotate (Putar Berlawanan Jarum Jam)</option>
                            <option value="Arc Shot (Gerakan Melengkung)">Arc Shot (Gerakan Melengkung)</option>
                        </select>
                        <input type="text" id="camera-movement-other" class="input-field other-input hidden" placeholder="Tuliskan gerakan kamera...">
                    </div>
                </div>
            </section>

            <!-- Bagian Negative Prompt -->
            <section class="form-section negative-section">
                <h2 class="form-section-title">⚠️ Negative Prompt</h2>
                <div class="input-container">
                    <label for="negative-prompt">Hindari elemen-elemen berikut:</label>
                    <textarea id="negative-prompt" class="textarea-field" rows="6">Teks, Subtitle, Logo, Distorsi, Artefak, Wajah Ganda, Cacat, Tangan Tidak Normal, Orang Tambahan, Objek Mengganggu, Kualitas Rendah, Buram, Glitch, Suara Robotik, Abstrak</textarea>
                </div>
            </section>
            
            <button id="generate-btn" class="btn btn-primary w-full text-lg">Buat Prompt!</button>

            <!-- Bagian Output -->
            <div id="output-container" class="hidden">
                <h2 class="form-section-title">Prompt yang Dihasilkan</h2>
                <textarea id="prompt-output" readonly></textarea>
                <div class="text-center mt-4">
                    <button id="copy-btn" class="btn btn-secondary">Salin Teks Prompt</button>
                </div>
            </div>

        </main>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Data untuk mengisi dropdown (termasuk preset baru dan yang sudah ada)
            const characterPresets = {
                pria_atletis_kaos_hitam: { gender: 'Laki-Laki', body: 'Postur tubuh tegap dan proporsional. Lengan terlihat berotot ringan. Bahu lebar. Tinggi badan di atas rata-rata.', skin: 'Bersih dan sehat.', face: 'Bentuk wajah oval dengan garis rahang yang tegas. Kulit tampak bersih dan sehat. Alis rapi dan mata tajam, menatap langsung ke kamera. Hidung lurus, bibir penuh dengan senyum tipis.', hair: 'Hitam pendek, ditata rapi ke atas', expression: 'Percaya diri, menatap kamera.', top: "Kaos hitam tulisan 'SOBAT KERE' putih", bottom: '', accessory: '' },
                wanita_anggun_kaos_biru: { gender: 'Perempuan', body: 'Ramping dan proporsional. Postur tegak, anggun dan tenang. Kaki jenjang, lengan ramping.', skin: 'Cerah dan bersih.', face: 'Oval dengan dagu runcing lembut. Mata sedikit menunduk. Bibir kecil, senyum tipis.', hair: 'Hitam pekat, panjang lurus', breasts: 'Sedang', expression: 'Lembut, damai, manis.', top: "Kaos putih tulisan 'SOBAT KERE' biru", bottom: 'Celana panjang ketat hitam', accessory: 'Memegang bunga kecil.' },
                wanita_ramping_tanktop_putih: { gender: 'Perempuan', body: 'Terlihat ramping dan proporsional, dengan tinggi badan sedang hingga tinggi. Bahu simetris dan tegap, lengan langsing dan halus. Pinggang tampak ramping dan tidak menonjol, menunjukkan postur fit dan terawat.', skin: 'Cerah dan mulus, dengan undertone hangat.', face: 'Wajah oval simetris. Kulit halus, cerah, dengan tone natural merata. Mata besar dan ekspresif, kelopak tegas. Alis rapi melengkung alami. Hidung kecil dan proporsional. Bibir penuh dan merona natural.', hair: 'Hitam panjang lurus, tampak lembut mengkilap.', breasts: 'Sedang hingga Besar', expression: 'Netral ke arah lembut, tenang, dan kalem.', top: "Tank top putih ketat", bottom: '', accessory: '' },
                wanita_elegan_rambut_coklat: { gender: 'Perempuan', body: 'Postur tegap dan ramping, dengan siluet seimbang dan elegan. Bahu proporsional, lengan langsing. Pinggang ramping memberikan siluet jam pasir ringan.', skin: 'Cerah dan halus, tampilan bersih dan merata.', face: 'Wajah oval lembut. Kulit cerah dan halus dengan rona alami. Mata besar dan bersinar, ekspresi tenang dan ramah. Alis rapi alami. Hidung kecil dan proporsional. Bibir tipis ke sedang, sedikit senyum manis.', hair: 'Coklat panjang bergelombang ringan', breasts: 'Sedang', expression: 'Tenang, ramah, dan daya tarik alami.', top: "Tank top putih transparan ringan", bottom: '', accessory: '' },
                pria_kasual_sawo_matang: { gender: 'Laki-Laki', body: 'Postur tegap dan tinggi sedang, tubuh aktif dan sehat. Bahu lurus dan cukup lebar. Lengan cukup berotot tapi ramping. Dada & pinggang fit dan proporsional.', skin: 'Coklat sawo matang, khas kulit tropis.', face: 'Wajah oval ke arah persegi, ramah. Mata ukuran sedang, ekspresif. Alis tebal alami. Hidung proporsional. Bibir sedang dengan senyuman kecil yang ceria.', hair: 'Hitam pekat, ditata rapi ke atas gaya modern.', expression: 'Ceria, hangat, dan santai.', top: 'Kaos abu-abu polos', bottom: 'Jeans robek bagian lutut', accessory: '', action: 'Berdiri santai di pematang sawah' },
                pria_kaukasian_artistik: { gender: 'Laki-Laki', etnis: 'Kaukasia', body: 'Tinggi dan ramping, sosok atletis ringan (awal 20-an). Bahu sedang dan sempit. Lengan panjang dan ramping. Dada & perut fit namun tidak berotot.', skin: 'Putih cerah merata.', face: 'Wajah oval sedikit tirus, rahang lembut namun tegas. Mata sedang dan dalam. Alis gelap dan tebal alami. Hidung lurus dan tajam. Bibir sedang, ekspresi netral.', hair: 'Coklat gelap, gaya semi berantakan, menyisir ke belakang alami.', expression: 'Kalem, cerdas, sedikit misterius.', top: 'Kaos putih polos', bottom: 'Celana panjang hitam slim fit', accessory: '', action: 'Berdiri santai di petak sawah tergenang, latar matahari terbenam.' },
                wanita_klasik_gaun_putih: { gender: 'Perempuan', body: 'Postur ramping dan tegap, gerakan anggun dan tenang. Bahu ramping dan lembut. Lengan langsing dan halus. Pinggang dan pinggul proporsional dengan lekuk lembut.', skin: 'Putih bersih dan merata, sangat terawat.', face: 'Wajah oval sempurna, garis rahang halus. Kulit putih pucat cerah dengan rona pipi kemerahan. Mata besar dan tenang. Alis tebal alami, melengkung halus. Hidung kecil dan mancung. Bibir penuh dan halus, sedikit mengatup.', hair: 'Coklat gelap panjang dan halus, tergerai alami.', breasts: 'Proporsional', expression: 'Tenang, dalam, misterius, memikat, berwibawa.', top: 'Gaun putih panjang bergaya klasik dengan kain menjuntai', bottom: '', accessory: 'Selempang', action: 'Berdiri di tengah hamparan sawah hijau, dalam cahaya senja.' },
                pria_sporty_kaos_biru: { gender: 'Laki-Laki', body: 'Tubuh proporsional dengan postur tegak dan tegap. Bahu cukup lebar, lengan ramping namun berisi. Tidak terlalu berotot, menunjukkan bentuk tubuh sehat dan aktif. Tinggi badan terlihat cukup (sekitar menengah hingga tinggi).', face: 'Bentuk wajah oval sedikit membulat. Alis tebal dan rapi, mata cukup besar dan fokus. Hidung lurus dan bibir sedang.', hair: 'pendek, hitam, dan tersisir rapi ke samping', top: 'Kaos oblong sporty dua warna: bagian tengah putih, lengan dan kerah biru muda. Di bagian dada terdapat tulisan "SOBAT KERE" dalam huruf kapital hitam.', expression: 'netral cenderung serius, sedang melihat ke arah atas' },
                wanita_anggun_bunga_sk: { gender: 'Perempuan', body: 'Tubuh ramping dan proporsional. Postur tegak, memberikan kesan anggun dan tenang. Kaki jenjang dan lurus, memberi kesan tinggi semampai. Lengan ramping dengan pose santai di samping tubuh.', face: 'Bentuk wajah oval dengan dagu runcing lembut. Kulit wajah cerah dan bersih. Mata sedikit menunduk. Bibir kecil dan tersenyum tipis.', hair: 'panjang, hitam, tergerai ke belakang bahu', expression: 'kalem, lembut dan damai, manis dan feminin', top: 'Kaos putih dengan tulisan besar berwarna biru: "SOBAT KERE" berdesain artistik dan santai.', bottom: 'Celana panjang ketat berwarna hitam', accessory: 'Tangan kiri memegang bunga kecil', action: 'Tidak mengenakan alas kaki (telanjang kaki), menyatu dengan suasana alam.' },
                wanita_fit_tanktop_hitam: { gender: 'Perempuan', body: 'Tubuh ramping dan fit, dengan lekuk yang proporsional. Postur tegap. Lengan ramping dan pinggang terlihat kecil. Kaki jenjang dan kokoh.', face: 'Bentuk wajah oval dengan dagu tegas. Alis tebal rapi, mata tajam dan fokus. Bibir penuh.', hair: 'panjang, hitam, digerai ke bawah dan sebagian mengarah ke depan bahu', expression: 'tenang dan sedikit serius, sedang menoleh ke samping kiri', top: 'Tanktop hitam tanpa lengan, ketat dan sederhana', bottom: 'celana pendek jeans biru gelap model high-waist', action: 'berdiri dengan percaya diri di tengah hutan. Tidak mengenakan alas kaki.' },
                wanita_damai_kaos_biru_sk: { gender: 'Perempuan', body: 'Tubuh ramping dan tinggi proporsional. Postur berdiri tegak dengan posisi tangan rileks. Lengan dan kaki tampak langsing. Bahu sempit dan pinggang kecil.', face: 'Wajah oval. Mata menunduk ke arah bunga. Alis hitam tebal, bibir kecil dan tersenyum tipis.', hair: 'panjang hitam, dikuncir rendah ke belakang', expression: 'lembut, tenang, kontemplatif atau damai', top: 'Kaos putih dengan desain tulisan tebal berwarna biru: "SOBAT KERE" bergaya artistik.', bottom: 'Celana panjang ketat hitam (legging)', accessory: 'Jam tangan di tangan kanan. Tangan kiri memegang bunga berwarna ungu muda.', action: 'Tidak mengenakan alas kaki, selaras dengan nuansa alami.' },
                wanita_kasual_kemeja_garis: { gender: 'Perempuan', body: 'Tegak dan proporsional. Tampak ramping dengan lekuk tubuh halus dan natural.', face: 'Wajah oval, dengan rahang halus dan dagu sedikit runcing. Alis tebal sedang, mata besar, hidung proporsional, bibir penuh. Kulit cerah dan merata.', hair: 'Hitam panjang, lurus atau sedikit bergelombang, terurai bebas.', expression: 'tenang dan percaya diri', top: "Kemeja lengan panjang bergaris biru-putih dengan dalaman tank top putih", bottom: 'Celana berwarna cokelat karamel pinggang tinggi' },
                wanita_minimalis_rok_putih: { gender: 'Perempuan', body: 'Ramping, proporsional, pinggang kecil, bahu dan pinggul seimbang. Lengan panjang dan ramping. Tinggi sedang hingga tinggi.', face: 'Wajah oval, kontur lembut dan seimbang. Alis hitam alami, mata besar berbentuk almond, ekspresi tajam namun tenang. Hidung ramping, lurus. Pipi lembut sedikit tirus. Bibir penuh. Rahang tidak tegas, dagu bulat lembut.', hair: 'Hitam pekat, panjang, lurus (sedikit gelombang alami), tergerai bebas.', expression: 'Cerah, ramah, hangat, bersahabat', top: 'Kaus putih polos bahan ribbed knit', bottom: 'Rok panjang atau midi putih flowy', action: 'Tangan bersedekap' },
                pria_edgy_jeans_robek: { gender: 'Laki-Laki', body: 'Atletis ramping. Lengan kencang, bahu lebar. Tinggi sedang hingga tinggi.', skin: 'Sawo matang alami', face: 'Oval ke persegi, rahang tegas. Alis hitam, lurus tebal. Mata sedang, ekspresi cerah dan ramah. Hidung lurus. Bibir penuh, tersenyum.', hair: 'Hitam pekat, dipotong pendek dan ditata dengan volume tinggi di bagian atas (gaya quiff atau pompadour ringan).', expression: 'Hangat, bersahabat, percaya diri.', top: 'Kaos oblong sederhana warna abu-abu polos', bottom: 'Celana jeans panjang sobek (ripped jeans) warna biru denim pudar, digulung sedikit.', accessory: 'Gelang hitam di tangan kanan.', action: 'Berjalan di tengah pematang sawah, tanpa alas kaki.' },
                wanita_elegan_kaos_putih: { gender: 'Perempuan', body: 'Ramping dan proporsional. Postur tegak. Bahu sempit, pinggang kecil. Tinggi sedang hingga tinggi.', face: 'Oval sempurna. Kulit cerah, bersih, mulus. Alis rapi natural. Mata besar, simetris, ekspresif. Hidung kecil, mancung. Bibir penuh, merah alami.', hair: 'Panjang, hitam pekat, lurus hingga sedikit bergelombang alami, tergerai rapi.', expression: 'Tenang, percaya diri, elegan.', top: 'Kaos pendek putih polos, slim fit', bottom: 'Bawahan berwarna gelap' },
                pria_pompadour_jeans_robek: { gender: 'Laki-Laki', body: 'Ramping dan atletis ringan. Dada dan bahu cukup lebar. Lengan panjang dan ramping. Tinggi sedang hingga tinggi.', skin: 'Sawo matang, bersih, dan sehat.', face: 'Persegi panjang dengan garis rahang tegas. Alis tebal dan lurus. Mata sedang, tajam namun ramah. Hidung proporsional. Bibir tipis ke sedang, senyum ramah.', hair: 'Hitam, pendek, dengan gaya pompadour pendek atau slicked-up.', expression: 'Penuh percaya diri, ramah.', top: 'Kaos oblong lengan pendek warna abu-abu polos', bottom: 'Celana jeans slim fit biru pudar dengan robekan di lutut, digulung ke atas.', accessory: 'Gelang hitam sederhana di pergelangan tangan kanan.', action: 'Berdiri di pematang sawah, tidak memakai alas kaki.' },
                wanita_croptop_pink: { gender: 'Perempuan', body: 'Ramping dan proporsional. Bahu terbuka. Dada cukup penuh. Pinggang ramping dan kecil. Postur tegap. Lengan ramping.', face: 'Oval. Kulit cerah dengan rona kemerahan. Mata cukup besar dan tajam. Alis tertata rapi, tebal natural. Hidung ramping. Bibir penuh, warna natural kemerahan.', hair: 'Panjang, lurus ke bergelombang halus, warna hitam gelap, dibiarkan terurai.', expression: 'Fokus, percaya diri, hangat.', top: 'Tank top crop merah muda pucat dengan empat kancing dan simpul pita.', accessory: 'Kalung rantai tipis dengan liontin kecil. Anting mungil.' },
                wanita_natural_rambut_coklat: { gender: 'Perempuan', body: 'Postur tegap dan proporsional. Bahu ramping. Dada terlihat berisi. Pinggang langsing (bentuk jam pasir).', face: 'Oval dan simetris. Kulit cerah dan halus. Mata besar, ekspresif, bulu mata lentik, alis tegas. Hidung mancung. Bibir penuh, merah natural.', hair: 'Panjang, tergerai alami, berwarna cokelat gelap dengan highlight.', expression: 'Natural dan menarik.', top: 'Atasan putih tipis dengan dalaman crop top putih.' },
                wanita_fit_rambut_coklat: { gender: 'Perempuan', body: 'Tinggi sedang hingga tinggi, ramping dan proporsional. Bahu dan lengan langsing. Dada sedang. Pinggang ramping, perut datar. Pinggul seimbang.', face: 'Oval. Kulit cerah dan mulus. Alis rapi, mata sedang berbentuk almond. Hidung lurus. Bibir sedang.', hair: 'Panjang, lurus, berwarna cokelat terang hingga keemasan.', expression: 'Kalem dan percaya diri.' }
            };
            const fullCharacterPresets = {
                "wanita_sporty_ekor_kuda": {
                    face: "Memiliki bentuk wajah oval dengan kulit yang halus dan riasan ringan namun rapi. Alisnya rapi dan tegas, matanya besar dengan eyeliner yang mempertegas bentuknya. Bibirnya penuh dengan warna natural.",
                    hair: "berwarna coklat gelap, mengikat ekor kuda tinggi dengan ikat rambut emas, memberi kesan segar dan sporty.",
                    top: "Mengenakan kaus crop hitam ketat dengan tulisan putih \"SOBAT KERE\" di bagian dada. Potongan kaus menampilkan bagian perut.",
                    body: "Terlihat memiliki tubuh langsing dan berlekuk, dengan postur tubuh tegap dan proporsional."
                },
                "wanita_feminin_ponytail": {
                    face: "Memiliki bentuk wajah oval dengan fitur halus dan simetris. Kulitnya tampak mulus dan bercahaya. Riasan wajah terlihat natural namun mempertegas kecantikannya, dengan alis rapi, eyeliner halus, bulu mata lentik, dan bibir berwarna lembut (nude pink).",
                    hair: "Warna cokelat gelap, diikat ke belakang dengan gaya ponytail tinggi menggunakan ikat rambut berwarna emas. Beberapa helai rambut dibiarkan menjuntai di sisi wajah, menambah kesan feminin.",
                    top: "Mengenakan crop top hitam ketat dengan tulisan putih besar bertuliskan \"SOBAT KERE\" , yang dalam bahasa Indonesia secara harfiah berarti \"teman miskin\", biasanya digunakan secara santai, ironis, atau humoris.",
                    body: "Tubuh ramping dan fit dengan perut rata yang terlihat jelas. Proporsi tubuh tampak seimbang dan posturnya tegak, mencerminkan kepercayaan diri."
                },
                "pria_serius_di_hutan": {
                    face: "Pria dengan ekspresi serius atau merenung, sedang menatap ke atas. Memiliki rahang tegas, rambut hitam pendek dan rapi, serta penampilan yang bersih dan maskulin.",
                    top: "Mengenakan kaus hitam dengan tulisan putih \"SOBAT KERE\". Kaus berukuran pas dan dipadukan dengan celana gelap.",
                    bottom: "Celana gelap.",
                    accessory: "Di pergelangan tangan kiri terlihat mengenakan jam tangan hitam.",
                    body: "Tubuh tegap dan proporsional, dengan postur berdiri tegak. Tingginya tampak sedang hingga tinggi.",
                    setting: "Berada di tengah hutan dengan pepohonan tinggi dan rapat, serta lantai hutan dipenuhi tanaman hijau. Cahaya matahari menembus dari sela-sela daun, menciptakan suasana alami dan tenang."
                },
                "wanita_anggun_kain_putih": {
                    face: "Wajahnya oval dengan fitur halus dan simetris. Ekspresi wajah tenang dan lembut.",
                    hair: "Rambut panjang, hitam, dan bergelombang, dibiarkan terurai dengan rapi di bahu dan punggung.",
                    body: "Tubuh terlihat langsing dan proporsional. Bahu ramping dan lengan atas tampak halus. Postur tubuh tegap namun santai.",
                    top: "Ia mengenakan kain putih polos yang dililitkan di tubuh, menyerupai gaya balutan toga atau kain tradisional. Kain tersebut menutupi tubuh dari bagian dada ke bawah, tanpa lengan atau detail tambahan.",
                    action: "Tampak kain tersebut dipegang di bagian depan dengan satu tangan, memberikan kesan sederhana dan anggun."
                },
                "pria_kasual_kaos_biru": {
                    face: "Wajah pria ini berbentuk oval dengan ekspresi tenang.",
                    hair: "Rambut hitam, pendek, dan ditata rapi ke atas dengan gaya modern dan bersih.",
                    body: "Postur tubuh proporsional dan tegap.",
                    top: "Mengenakan kaus oblong putih dengan tulisan besar berwarna biru bertuliskan: \"SOBAT KERE\" dan simbol huruf K besar di bawahnya.",
                    bottom: "Celana panjang berwarna abu-abu tua atau gelap. Potongan celananya tampak lurus (straight cut) dan fit di badan. Bahan celana terlihat seperti kain kasual (kemungkinan katun atau bahan sejenis).",
                    accessory: "Jam tangan berwarna hitam di pergelangan tangan kiri.",
                    action: "Lengan terlihat santai dengan tangan dimasukkan ke saku celana."
                },
                "pria_boots_coklat": {
                    face: "Bentuk wajah: Oval dengan rahang yang tidak terlalu tegas, proporsional dan simetris. Ekspresi wajah: Netral hingga sedikit serius, dengan pandangan mengarah ke samping kanan (dari sudut pandang kamera). Fitur: Alis tegas, hidung lurus, dan dagu tidak menonjol — wajah yang bersih tanpa aksesori seperti kacamata atau topi.",
                    hair: "Pendek, hitam, dengan potongan rapi dan sedikit disisir ke atas (gaya modern minimalis).",
                    body: "Postur tubuh: Tegap dan proporsional. Tinggi badan terlihat ideal dan tubuh cenderung slim atau sedang (tidak terlalu kurus atau berotot). Bahu lebar dan lengan ramping, menunjukkan tubuh yang fit.",
                    top: "Kaos oblong berwarna hitam. Terdapat tulisan besar di bagian depan dengan font tebal berwarna kuning emas bertuliskan: \"SOBAT KERE\".",
                    bottom: "Celana jeans biru dengan gaya slim fit. Terdapat gradasi warna pudar di bagian lutut dan paha. Dipadukan dengan sepatu boots berwarna cokelat muda (tan/brown) model tinggi di pergelangan kaki.",
                    accessory: "Jam tangan hitam di pergelangan tangan kiri."
                },
                 "pria_kaos_hitam_sk": {
                    body: "Pria dengan postur tinggi sedang hingga tinggi. Bentuk tubuh proporsional, tidak terlalu kurus maupun berotot — terlihat fit dan ramping. Posisi berdiri tegak dengan bahu rileks, memberi kesan percaya diri.",
                    face: "Wajah oval dengan rahang yang cukup tegas. Kulit sawo matang cerah. Alis tebal alami, mata tampak tajam namun tenang. Ekspresi wajah kalem dan fokus, memandang ke arah samping atas.",
                    hair: "Rambut hitam pekat dan disisir rapi ke samping.",
                    top: "Mengenakan kaus hitam dengan tulisan besar berwarna putih bertuliskan: \"SOBAT KERE\". Kaus berpotongan biasa, lengan pendek, dan pas di badan tanpa terlalu ketat.",
                    bottom: "Memakai celana panjang hitam (kemungkinan berbahan jeans atau chino). Celana fit/slim di bagian kaki, memberi kesan modern dan rapi."
                },
                "wanita_duduk_santai": {
                    body: "Postur tinggi dan langsing. Tubuh tampak proposional dan sehat. Bahu tegap dan pinggang ramping, menambah kesan elegan dan percaya diri.",
                    face: "Wajah oval dengan kontur lembut. Kulit cerah dan bersih. Alis rapi, mata tampak tenang dan lembut, menghadap ke bawah. Riasan ringan dan natural, menampilkan kesan anggun dan kalem.",
                    hair: "Rambut cokelat terang, ditata rapi dalam model kepang samping yang stylish.",
                    top: "Kaos putih dengan tulisan biru besar: \"SOBAT KERE\", menciptakan kesan santai dan sedikit jenaka. Potongan kaos sederhana namun pas di tubuh, memberikan tampilan kasual yang bersih.",
                    bottom: "Memakai jeans biru high-waist yang pas badan, potongan klasik. Celana menonjolkan bentuk pinggang ramping dan kaki panjang, memperkuat kesan kasual elegan."
                },
                 "wanita_kaos_putih_oversized": {
                    body: "Postur tubuh proporsional dan ramping. Tinggi sedang dengan bentuk tubuh yang feminim dan seimbang. Duduk menyamping di jalan setapak dengan satu kaki disilangkan, memberi kesan santai dan percaya diri.",
                    face: "Wajah oval dengan fitur yang halus dan simetris. Kulit cerah, mulus, dan bercahaya alami. Alis rapi, mata besar dan ekspresif. Bibir tampak memakai lipstik merah natural yang menonjolkan kesan segar dan anggun. Ekspresi wajah lembut dan bersahabat.",
                    hair: "Rambut panjang lurus berwarna hitam pekat, dibiarkan terurai rapi.",
                    top: "Mengenakan kaus putih polos, model oversized ringan namun tetap rapi. Lengan pendek, nyaman untuk suasana santai di alam terbuka. Bagian bawah kaus sedikit masuk ke celana, memberikan kesan kasual yang teratur.",
                    bottom: "Memakai celana panjang skinny fit hitam, berbahan kemungkinan denim atau katun stretch. Celana memberi kesan ramping dan modern, serasi dengan kaus putih polos."
                },
                "wanita_bra_hitam_kepang": {
                    gender: "Perempuan",
                    body: "Bentuk tubuh yang ramping dan proporsional, dengan pinggang yang terlihat kecil dan lengan yang langsing.",
                    face: "Wajahnya berbentuk oval dengan kulit cerah dan mulus. Ekspresi wajah netral atau sedikit tersenyum. Ia memiliki mata yang besar, hidung kecil, dan bibir yang penuh.",
                    hair: "Rambut panjang, hitam, dan dikepang ke samping. Tampak lurus dan halus, dengan sedikit kilau alami dan volume cukup tebal.",
                    top: "Bra berwarna hitam tanpa tambahan pakaian luar.",
                    bottom: "Celana jeans berwarna biru tua."
                },
                "wanita_kargo_biru_rambut_lurus": {
                    gender: "Perempuan",
                    body: "Tubuh ramping dan tinggi, dengan postur tegak. Pinggang kecil dan perut rata, memberi kesan tubuh proporsional. Lengan dan kaki terlihat jenjang.",
                    face: "Bentuk wajah oval. Kulit cerah dan mulus. Mata besar dan ekspresif. Hidung kecil dan lurus. Bibir penuh, dengan ekspresi wajah tenang atau sedikit serius.",
                    hair: "Warna hitam pekat, panjang menjuntai hingga bagian bawah punggung. Gaya lurus dan tergerai bebas, tampak halus dan berkilau alami.",
                    top: "Bra atau crop top berwarna biru muda, dengan tali tipis dan model sederhana.",
                    bottom: "Celana panjang model kargo berwarna biru tua, dengan kantong besar di samping dan potongan longgar."
                },
                "wanita_dress_bodycon_putih": {
                    gender: "Perempuan",
                    body: "Tubuh ramping dan proporsional. Pinggang kecil, lekuk tubuh terlihat jelas. Postur tubuh tegak dan elegan saat berjalan.",
                    face: "Wajah berbentuk oval dengan kulit cerah dan halus. Mata besar dan bersinar. Bibir penuh dengan ekspresi tenang dan sedikit tersenyum. Gaya makeup tampak natural dan rapi.",
                    hair: "Rambut hitam, panjang mencapai area perut, lurus, tergerai bebas, dan tampak rapi.",
                    top: "Dress bodycon putih berlengan tiga perempat (menyatu dengan bawahan).",
                    bottom: "(Bagian dari dress)",
                    accessory: "Sepatu hak tinggi warna nude/pink muda."
                },
                "wanita_kaos_putih_natural": {
                    gender: "Perempuan",
                    body: "Proporsional dan ramping.",
                    face: "Bentuk wajah oval dengan kulit cerah dan mulus. Mata cukup besar dan ekspresif. Bibir penuh dan tampak lembut, dengan sedikit senyum alami. Makeup sangat natural.",
                    hair: "Warna hitam gelap, lurus, panjang melewati dada, dan terurai rapi alami dengan kilau sehat.",
                    top: "Kaos berwarna putih polos, model lengan pendek dengan lipatan kecil di bagian ujung lengan.",
                    bottom: ""
                },
                "wanita_poni_lurus_bra_ungu": {
                    gender: "Perempuan",
                    body: "Proporsional dan ramping.",
                    face: "Bentuk wajah oval dengan kontur lembut. Kulit cerah dan mulus. Ekspresi tenang dan kalem. Makeup sangat natural atau minimal.",
                    hair: "Warna hitam pekat, gaya lurus panjang jatuh bebas di atas bahu, dilengkapi poni lurus yang menutupi dahi.",
                    top: "Bra berwarna ungu muda (lavender) dengan detail pita kecil di tengah.",
                    bottom: "Celana panjang berwarna biru tua (navy) dengan potongan lurus dan longgar."
                },
                "wanita_gaun_putih_strapless": {
                    gender: "Perempuan",
                    body: "Ramping dan proporsional.",
                    face: "Bentuk wajah oval dengan rahang halus. Kulit cerah dan tampak mulus. Ekspresi anggun dan tenang, dengan pandangan sedikit menyamping. Makeup lembut dan feminin.",
                    hair: "Warna hitam pekat, panjang dan bergelombang, dibiarkan terurai secara alami dengan volume tebal.",
                    top: "Gaun panjang tanpa lengan berwarna putih, potongan strapless (tanpa tali) mengalir sampai ke tanah.",
                    bottom: "(Bagian dari gaun)",
                    accessory: "Memberi kesan romantis, etereal, dan klasik."
                },
                "wanita_bra_top_transparan": {
                    gender: "Perempuan",
                    body: "Tubuh proporsional dengan postur tegak. Pinggang ramping dan bahu simetris. Lengan ramping dan terlihat sehat. Penampilan keseluruhan menunjukkan bentuk tubuh langsing dan atletis.",
                    face: "Bentuk wajah oval. Kulit wajah halus dan cerah. Bibir penuh dan simetris. Hidung kecil dan proporsional. Mata besar dengan riasan yang menonjolkan bentuknya.",
                    hair: "Rambut panjang, lurus, berwarna hitam gelap, dibiarkan tergerai",
                    top: "Mengenakan atasan dengan model bra-top berwarna putih atau krem. Potongan bagian atas cukup terbuka, memperlihatkan bahu dan belahan dada. Bahan tipis dan transparan mulai dari bawah dada hingga pinggang.",
                    bottom: "Rok tipis dan transparan, menyatu dengan bagian atas seperti dress. Model rok panjangnya tidak rata, terdiri dari kain tipis yang terbuka di tengah dan sedikit terbagi ke samping. Terdapat lapisan dalam pendek (mirip celana pendek) untuk menutupi bagian vital."
                },
                "wanita_kimono_putih_biru": {
                    gender: "Perempuan",
                    body: "Tubuh ramping dengan postur tegap dan anggun. Proporsi tubuh tampak seimbang, meskipun sebagian besar tubuh tertutupi pakaian longgar. Gestur tangan lembut dan tenang, menunjukkan sikap kalem.",
                    face: "Wajah berbentuk oval dengan kontur halus. Kulit cerah dan bersih. Alis rapi, mata besar dan tenang dengan ekspresi damai. Hidung kecil dan proporsional. Bibir penuh dengan senyuman samar.",
                    hair: "Rambut lurus, hitam, panjang sebahu, tergerai alami.",
                    breasts: "Karena pakaian yang longgar dan tidak memperlihatkan lekuk tubuh secara eksplisit, bentuk dan ukuran dada tidak tampak jelas. Siluet tubuh bagian atas tidak menunjukkan tonjolan signifikan, menekankan kesan sederhana dan sopan.",
                    top: "Mengenakan pakaian tradisional mirip yukata atau kimono ringan berwarna putih dengan motif bunga biru. Lengan panjang dan lebar, menjuntai ke bawah dengan gaya khas pakaian Jepang atau Asia Timur lainnya. Potongan bagian atas menutupi seluruh tubuh dari leher hingga bawah perut, sangat tertutup dan anggun."
                },
                "wanita_dress_bodycon_vneck": {
                    gender: "Perempuan",
                    body: "Tubuh ramping dan tinggi dengan postur tegap. Pinggang kecil dan proporsional terhadap bahu dan pinggul. Siluet tubuh terlihat elegan karena pakaian yang ketat menonjolkan lekuk tubuh secara halus.",
                    face: "Wajah berbentuk oval dengan garis wajah halus. Kulit cerah dan mulus. Mata besar dan ekspresif, memberi kesan tenang. Bibir berbentuk simetris dengan riasan natural.",
                    hair: "Rambut panjang dikepang ke samping, menambah kesan feminin dan klasik.",
                    breasts: "Terlihat proporsional dan natural. Terdefinisi namun tidak terlalu menonjol berkat model pakaian yang menyatu dengan bentuk tubuh.",
                    top: "Mengenakan dress bodycon berwarna putih dengan potongan leher berbentuk V. Lengan panjang hingga siku, memberikan kesan elegan dan rapi. Bahan pakaian elastis, mengikuti bentuk tubuh.",
                    bottom: "Merupakan kelanjutan dari gaun yang sama, jatuh panjang hingga ke mata kaki. Model lurus (slim fit) tanpa lipatan atau aksen tambahan. Tidak ada belahan terbuka, memperkuat kesan formal dan anggun."
                },
                "wanita_gaun_wrap_putih": {
                    gender: "Perempuan",
                    body: "Proporsi tubuh langsing dan tinggi. Bahu sejajar dengan pinggul, menciptakan siluet yang seimbang. Pinggang ramping, mempertegas lekuk tubuh secara elegan. Postur tubuh tampak anggun dan tegak.",
                    face: "Bentuk wajah oval dengan rahang lembut. Kulit halus dan cerah, tampak natural. Mata besar dan ekspresif, riasan mata ringan namun mempertegas sorot mata. Hidung ramping, bibir penuh dengan warna natural.",
                    hair: "Rambut panjang dikepang ke samping, menciptakan kesan feminin dan klasik.",
                    breasts: "Ukuran tampak sedang dan proporsional. Model pakaian memperlihatkan bentuk namun tetap sopan, dengan potongan leher V yang membingkai area dada secara halus.",
                    top: "Gaun putih model wrap (silang) di bagian dada, dengan potongan leher V yang elegan. Lengan panjang hingga siku, ketat namun tetap nyaman dilihat. Bahan gaun tampak lembut dan lentur, mengikuti kontur tubuh.",
                    bottom: "Merupakan bagian bawah dari gaun yang sama, model panjang hingga mata kaki. Potongan lurus mengikuti bentuk tubuh, menciptakan kesan anggun dan ramping. Tidak terdapat belahan atau ornamen tambahan—desainnya minimalis dan elegan."
                },
                "wanita_gaun_mini_puff": {
                    gender: "Perempuan",
                    body: "Tubuh ramping dengan postur tegap. Kaki jenjang dan proporsional, terlihat jelas karena pakaian pendek. Siluet tubuh menunjukkan keseimbangan antara bahu, pinggang, dan pinggul.",
                    face: "Bentuk wajah oval dengan garis rahang lembut. Kulit halus dan cerah. Mata besar dan tatapan tajam, dilengkapi dengan riasan mata ringan namun menonjolkan fitur. Bibir penuh, diberi sentuhan warna natural.",
                    hair: "Rambut panjang, terurai bebas hingga ke bawah dada, memberi kesan feminin dan anggun.",
                    breasts: "Ukuran tampak sedang dan proporsional. Pakaian dengan potongan leher V cukup dalam menonjolkan area dada dengan elegan namun tetap sopan.",
                    top: "Gaun mini putih dengan potongan wrap di bagian atas, membentuk leher V yang memperindah siluet. Lengan pendek menggembung (puff sleeves), memberi kesan lembut dan klasik.",
                    bottom: "Bagian bawah rok mengembang ringan dan berakhir di atas lutut, menciptakan tampilan muda, ringan, dan segar. Bahan gaun tampak ringan dan jatuh alami mengikuti gerakan tubuh.",
                    accessory: "Kalung besar dan mencolok, menambah kesan elegan dan dewasa. Sepatu hak tinggi hitam dengan desain tali, memberi kontras yang kuat dengan gaun putih. Gelang di tangan kiri sebagai sentuhan tambahan."
                },
                "wanita_mungil_rambut_pendek": {
                    gender: "Perempuan",
                    body: "Tubuh ramping dengan bentuk yang mungil dan proporsional. Postur tubuh tegak dan menunjukkan kepercayaan diri. Kaki terlihat kuat namun feminin, cocok dengan busana kasual yang dikenakan.",
                    face: "Bentuk wajah bulat ke oval, dengan pipi yang sedikit chubby memberi kesan muda dan manis. Kulit cerah dan mulus, memantulkan cahaya alami dengan baik. Senyum hangat dan tulus, memperkuat kesan ramah dan approachable. Mata cukup besar dan ekspresif, dengan alis rapi dan gaya riasan natural.",
                    hair: "Rambut pendek sebahu, lurus dan rapi, menciptakan tampilan segar dan modern.",
                    breasts: "Tampak berukuran kecil hingga sedang, proporsional dengan postur mungil. Tank top ketat tapi sopan menunjukkan bentuk alami tanpa menekankan secara eksplisit."
                },
                "wanita_curvy_dress_bodycon": {
                    gender: "Perempuan",
                    body: "Tubuh sangat proporsional dan curvy (berlekuk). Lekuk pinggul dan dada sangat menonjol, menciptakan siluet yang sensual dan tegas. Postur tubuh elegan, dengan posisi berdiri menyamping sedikit mempertegas bentuk tubuh.",
                    face: "Wajah oval, dengan fitur halus dan simetris. Kulit mulus dan cerah, mendukung kesan feminin dan bersih. Bibir penuh, dengan ekspresi wajah yang lembut namun sedikit menggoda. Mata tajam namun tetap lembut, memberi kesan confident tapi tenang.",
                    hair: "Rambut panjang bergelombang, tebal dan hitam, jatuh bebas hingga ke bawah punggung.",
                    top: "Mengenakan bodycon dress putih ketat dengan potongan sederhana. Gaun mempertegas lekuk tubuh secara maksimal, namun tetap terlihat rapi dan tidak berlebihan.",
                    bottom: "Tampilan berpadu antara kesan anggun dan sensual, cocok untuk tema pemotretan fashion atau elegan outdoor.",
                    breasts: "Payudara tampak berukuran besar, ditonjolkan dengan pakaian ketat yang dikenakan. Pinggul juga terlihat besar dan bulat, menambah kesan hourglass figure yang kuat. Perpaduan ini menciptakan bentuk tubuh yang sangat menonjolkan feminitas secara visual."
                },
                "wanita_hourglass_croptop_jeans": {
                    gender: "Perempuan",
                    body: "Tubuh ramping namun sangat berlekuk, menyerupai hourglass figure. Pinggang kecil, dada dan pinggul proporsional dan mencolok. Postur tubuh tegak, penuh percaya diri dengan satu tangan di saku, menciptakan kesan santai namun tegas.",
                    face: "Wajah oval dengan struktur rahang tegas namun tetap feminin. Kulit cerah dan halus, tanpa noda, memberi kesan segar dan bersih. Bibir penuh dan simetris, dipadukan dengan ekspresi wajah netral tapi mengesankan ketenangan dan kekuatan. Mata besar dengan riasan natural, fokus dan menawan.",
                    hair: "Rambut panjang bergelombang, hitam pekat, ditata rapi ke samping.",
                    top: "Mengenakan crop top putih dengan detail renda di bawah dan spaghetti straps, yang menonjolkan bentuk tubuh bagian atas secara signifikan.",
                    bottom: "Bawahan berupa celana jeans biru ketat dengan sobekan kecil di bagian paha, menambah kesan kasual namun modern.",
                    breasts: "Payudara terlihat besar dan penuh, sangat ditonjolkan oleh crop top yang dikenakan. Pinggul proporsional, dengan lekuk tubuh yang sangat jelas, memperkuat kesan curvy secara keseluruhan."
                },
                "wanita_artistik_hutan": {
                    gender: "Perempuan",
                    body: "Tubuh ramping dan tinggi, dengan postur elegan. Proporsi tubuh cenderung slim dan natural, tanpa lekuk mencolok. Gerakan dan posisi tubuh menggambarkan kelembutan dan keanggunan, lebih ke arah estetika klasik atau artistik.",
                    face: "Wajah oval, cenderung tirus dan bersih. Ekspresi wajah tenang, sedikit melamun atau kontemplatif. Alis lurus dan lembut, memberi kesan polos dan alami.",
                    hair: "Rambut pendek sebahu, potongan bob lurus, memberi kesan simpel dan artistik.",
                    top: "Mengenakan gaun panjang putih dengan lengan panjang. Gaya berpakaian ini memberi kesan anggun, minimalis, dan lembut, sangat cocok untuk suasana hutan yang dikelilingi cahaya alami.",
                    bottom: "Nuansa pakaian dan pose menciptakan efek visual seperti potret dari lukisan atau film indie."
                }
            };
            const fullPresetOptions = {
                "Wanita (Sobat Kere)": {
                    "wanita_sporty_ekor_kuda": "Wanita Sporty (Ekor Kuda)",
                    "wanita_feminin_ponytail": "Wanita Feminin (Ponytail)",
                    "wanita_anggun_kain_putih": "Wanita Anggun (Kain Putih)",
                    "wanita_duduk_santai": "Wanita Duduk Santai (Kepang Samping)",
                    "wanita_kaos_putih_oversized": "Wanita Santai (Kaos Putih Oversized)"
                },
                "Pria (Sobat Kere)": {
                    "pria_serius_di_hutan": "Pria Serius di Hutan (Kaos Hitam)",
                    "pria_kasual_kaos_biru": "Pria Kasual (Kaos Biru)",
                    "pria_boots_coklat": "Pria Boots Coklat (Kaos Emas)",
                    "pria_kaos_hitam_sk": "Pria Kalem (Kaos Hitam SK)"
                },
                "Wanita (Tambahan)": {
                    "wanita_bra_hitam_kepang": "Wanita Bra Hitam & Kepang Samping",
                    "wanita_kargo_biru_rambut_lurus": "Wanita Celana Kargo & Rambut Lurus",
                    "wanita_dress_bodycon_putih": "Wanita Dress Bodycon Putih",
                    "wanita_kaos_putih_natural": "Wanita Kaos Putih Natural",
                    "wanita_poni_lurus_bra_ungu": "Wanita Poni Lurus & Bra Ungu",
                    "wanita_gaun_putih_strapless": "Wanita Gaun Putih Strapless"
                },
                "Wanita (Gaun & Dress Lanjutan)": {
                    "wanita_bra_top_transparan": "Wanita (Bra-Top Transparan)",
                    "wanita_kimono_putih_biru": "Wanita (Kimono Putih-Biru)",
                    "wanita_dress_bodycon_vneck": "Wanita (Dress Bodycon V-Neck)",
                    "wanita_gaun_wrap_putih": "Wanita (Gaun Wrap Putih)",
                    "wanita_gaun_mini_puff": "Wanita (Gaun Mini Puff Sleeves)",
                    "wanita_artistik_hutan": "Wanita Artistik (Gaun Putih di Hutan)"
                },
                "Wanita (Gaya Beragam)": {
                     "wanita_mungil_rambut_pendek": "Wanita Mungil (Rambut Pendek)",
                     "wanita_curvy_dress_bodycon": "Wanita Curvy (Dress Bodycon)",
                     "wanita_hourglass_croptop_jeans": "Wanita Hourglass (Crop Top & Jeans)"
                }
            };
            const ageOptions = Array.from({length: 130}, (_, i) => `${i + 1}`);
            const skinOptions = ["Putih Bersih", "Putih Langsat", "Sawo Matang"];
            const breastOptions = ["Bulat Kecil", "Bulat Sedang", "Bulat Besar", "Bulat Sangat Besar"];
            const hairOptions = ["Hitam pekat, panjang lurus", "Hitam panjang, lurus/sedikit bergelombang", "Hitam pendek, ditata rapi ke atas", "Hitam pendek, tersisir rapi ke samping", "pendek, hitam, dan tersisir rapi ke samping", "panjang, hitam, tergerai ke belakang bahu", "panjang, hitam, digerai ke bawah dan sebagian mengarah ke depan bahu", "panjang hitam, dikuncir rendah ke belakang", "Hitam pekat, dipotong pendek dan ditata dengan volume tinggi di bagian atas (gaya quiff atau pompadour ringan)", "Hitam, pendek, dengan gaya pompadour pendek atau slicked-up", "Panjang, lurus ke bergelombang halus, warna hitam gelap, dibiarkan terurai", "Panjang, tergerai alami, berwarna cokelat gelap dengan highlight", "Panjang, lurus, berwarna cokelat terang hingga keemasan", "Cokelat panjang bergelombang ringan", "Cokelat terang keemasan, panjang lurus", "Cokelat gelap dengan highlight, panjang", "Hitam/Cokelat tua, panjang bergelombang", "Pirang Platinum", "Pirang Keemasan", "Merah Tembaga", "Merah Anggur", "Abu-abu/Silver", "Biru Tua", "Hijau Zamrud", "Ungu Lavender"];
            const topOptions = ["Kaos hitam tulisan 'SOBAT KERE' putih", "Kaos putih-biru tulisan 'SOBAT KERE' hitam", "Kaos putih tulisan 'SOBAT KERE' biru", "Kaos oblong sporty dua warna: bagian tengah putih, lengan dan kerah biru muda", "Tank top hitam ketat", "Tank top putih transparan ringan", "Tank top crop merah muda pucat dengan empat kancing dan simpul pita", "Atasan putih tipis dengan dalaman crop top putih", "Gaun off-shoulder pink motif bunga dengan renda", "Kemeja garis biru-putih & dalaman tank top putih", "Kaus putih ribbed knit", "Kaos putih polos", "Kaos abu-abu polos", "Gaun putih panjang bergaya klasik"];
            const bottomOptions = ["Celana panjang ketat hitam", "Celana panjang ketat hitam (legging)", "Celana pendek jeans biru gelap high-waist", "Celana cokelat karamel pinggang tinggi", "Rok panjang/midi putih flowy", "Bawahan berwarna gelap", "Rok Mini Hitam", "Rok Mini Putih", "Rok Pendek Hitam", "Rok Pendek Putih", "Celana Panjang Hitam", "Rok Panjang Hitam", "Celana Panjang Biru Muda", "Rok Panjang Biru Muda", "Celana Panjang Biru Tua", "Rok Panjang Biru Tua", "Jeans robek bagian lutut", "Celana panjang hitam slim fit"];
            const presetOptions = {
                "Pria (Sobat Kere)": { 
                    pria_atletis_kaos_hitam: "Pria Atletis (Kaos Hitam SK)",
                    pria_sporty_kaos_biru: "Pria Sporty (Kaos Biru SK)"
                },
                "Wanita (Sobat Kere)": { 
                    wanita_anggun_kaos_biru: "Wanita Anggun (Kaos Biru SK)",
                    wanita_anggun_bunga_sk: "Wanita Anggun Bunga (Kaos Biru SK)",
                    wanita_damai_kaos_biru_sk: "Wanita Damai (Kaos Biru SK)"
                },
                "Wanita (Umum)": {
                    wanita_ramping_tanktop_putih: "Wanita Ramping (Tank Top Putih)",
                    wanita_elegan_rambut_coklat: "Wanita Elegan (Rambut Coklat)",
                    wanita_klasik_gaun_putih: "Wanita Klasik (Gaun Putih)",
                    wanita_fit_tanktop_hitam: "Wanita Fit (Tank Top Hitam)",
                    wanita_kasual_kemeja_garis: "Wanita Kasual (Kemeja Garis)",
                    wanita_minimalis_rok_putih: "Wanita Minimalis (Rok Putih)",
                    wanita_elegan_kaos_putih: "Wanita Elegan (Kaos Putih)",
                    wanita_croptop_pink: "Wanita (Crop Top Pink)",
                    wanita_natural_rambut_coklat: "Wanita Natural (Rambut Coklat)",
                    wanita_fit_rambut_coklat: "Wanita Fit (Rambut Coklat)"
                },
                "Pria (Umum)": {
                    pria_kasual_sawo_matang: "Pria Kasual (Sawo Matang)",
                    pria_kaukasian_artistik: "Pria Artistik (Kaukasia)",
                    pria_edgy_jeans_robek: "Pria Edgy (Jeans Robek)",
                    pria_pompadour_jeans_robek: "Pria Pompadour (Jeans Robek)"
                }
            };
            const etnisOptions = ["Jawa", "Sunda", "Aceh", "Minang", "Dayak", "Madura"];
            const accentOptions = ["Jawa", "Sunda", "Aceh", "Minang", "Dayak", "Madura"];
            const voiceDescOptions = ["Jernih", "Serak", "Serak Basah", "Lembut", "Halus"];
            const accessoryOptions = ["Kalung Emas", "Jam Tangan"];

            // Fungsi untuk mengisi dropdown
            function populateSelect(element, options, hasOptGroups = false) {
                const isPreset = element.id.includes('preset');
                element.innerHTML = `<option value="">-- Pilih ${isPreset ? 'Preset' : 'Opsi'} --</option>`;
                if (hasOptGroups) {
                    for (const groupLabel in options) {
                        const optgroup = document.createElement('optgroup');
                        optgroup.label = groupLabel;
                        for (const [value, text] of Object.entries(options[groupLabel])) {
                            const option = document.createElement('option');
                            option.value = value;
                            option.textContent = text;
                            optgroup.appendChild(option);
                        }
                        element.appendChild(optgroup);
                    }
                } else {
                    options.forEach(opt => {
                        const option = document.createElement('option');
                        option.value = opt;
                        option.textContent = opt;
                        element.appendChild(option);
                    });
                }
                // Tambahkan opsi "Tulis Lainnya"
                const otherOption = document.createElement('option');
                otherOption.value = 'other';
                otherOption.textContent = 'Tulis Lainnya...';
                element.appendChild(otherOption);
            }

            // Fungsi untuk menangani pilihan "Tulis Lainnya"
            function handleOtherOption(event) {
                const selectElement = event.target;
                const otherInputElement = document.getElementById(selectElement.id + '-other');
                if (otherInputElement) {
                    if (selectElement.value === 'other') {
                        otherInputElement.classList.remove('hidden');
                    } else {
                        otherInputElement.classList.add('hidden');
                        otherInputElement.value = ''; // Kosongkan input jika opsi lain dipilih
                    }
                }
            }
            
            // Inisialisasi semua dropdown
            document.querySelectorAll('select').forEach(select => {
                const id = select.id;
                if (id.includes('-full-preset')) populateSelect(select, fullPresetOptions, true);
                else if (id.includes('-preset')) populateSelect(select, presetOptions, true);
                else if (id.includes('-hair')) populateSelect(select, hairOptions);
                else if (id.includes('-top')) populateSelect(select, topOptions);
                else if (id.includes('-bottom')) populateSelect(select, bottomOptions);
                else if (id.includes('-etnis')) populateSelect(select, etnisOptions);
                else if (id.includes('-accent')) populateSelect(select, accentOptions);
                else if (id.includes('-voice-desc')) populateSelect(select, voiceDescOptions);
                else if (id.includes('-accessory')) populateSelect(select, accessoryOptions);
                else if (id.includes('-age')) populateSelect(select, ageOptions);
                else if (id.includes('-skin')) populateSelect(select, skinOptions);
                else if (id.includes('-breasts')) populateSelect(select, breastOptions);
                else { // Untuk select yang opsinya sudah ada di HTML
                    const otherOption = document.createElement('option');
                    otherOption.value = 'other';
                    otherOption.textContent = 'Tulis Lainnya...';
                    select.appendChild(otherOption);
                }
                select.addEventListener('change', handleOtherOption);
            });
            
            // Fungsi untuk menerapkan preset
            function applyPreset(characterNumber, presetKey, presetData) {
                if (!presetKey || presetKey === 'other') return;
                const data = presetData[presetKey];
                if (!data) return;
                for (const [field, value] of Object.entries(data)) {
                    const element = document.getElementById(`c${characterNumber}-${field}`);
                    if (element) {
                        if (element.tagName === 'SELECT') {
                            const optionExists = [...element.options].some(opt => opt.value === value);
                            if (optionExists) {
                                element.value = value;
                                const otherInput = document.getElementById(element.id + '-other');
                                if (otherInput) {
                                    otherInput.classList.add('hidden');
                                    otherInput.value = '';
                                }
                            } else {
                                element.value = 'other';
                                const otherInput = document.getElementById(element.id + '-other');
                                if (otherInput) {
                                    otherInput.value = value;
                                    otherInput.classList.remove('hidden');
                                }
                            }
                        } else {
                            element.value = value || '';
                        }
                        element.dispatchEvent(new Event('change'));
                    }
                }
            }

            // Tambahkan event listener untuk semua preset dropdowns
            for (let i = 1; i <= 5; i++) {
                document.getElementById(`c${i}-preset`)?.addEventListener('change', (e) => applyPreset(i, e.target.value, characterPresets));
                document.getElementById(`c${i}-full-preset`)?.addEventListener('change', (e) => applyPreset(i, e.target.value, fullCharacterPresets));
            }

            // Fungsi untuk menampilkan/menyembunyikan section karakter
            function setupCharacterToggle(addBtnId, removeBtnId, sectionId) {
                const addBtn = document.getElementById(addBtnId);
                const removeBtn = document.getElementById(removeBtnId);
                const section = document.getElementById(sectionId);

                addBtn.addEventListener('click', () => {
                    section.classList.remove('hidden');
                    addBtn.classList.add('hidden');
                });

                removeBtn.addEventListener('click', () => {
                    section.classList.add('hidden');
                    section.querySelectorAll('input, select, textarea').forEach(el => {
                         if (el.tagName === 'SELECT') {
                            el.selectedIndex = 0;
                        } else {
                            el.value = '';
                        }
                        el.dispatchEvent(new Event('change'));
                    });
                    addBtn.classList.remove('hidden');
                });
            }
            
            // Fungsi untuk menampilkan/menyembunyikan section scene secara berurutan
            function setupSceneToggles() {
                const maxScenes = 6;
                for (let i = 2; i <= maxScenes; i++) {
                    const addBtn = document.getElementById(`add-scene-btn-${i}`);
                    const removeBtn = document.getElementById(`remove-scene-btn-${i}`);
                    const section = document.getElementById(`scene${i}-section`);
                    const nextAddBtn = document.getElementById(`add-scene-btn-${i + 1}`);

                    if (addBtn) {
                        addBtn.addEventListener('click', () => {
                            if (section) section.classList.remove('hidden');
                            addBtn.classList.add('hidden');
                            if (nextAddBtn) nextAddBtn.classList.remove('hidden');
                        });
                    }

                    if (removeBtn) {
                        removeBtn.addEventListener('click', () => {
                             // Sembunyikan scene saat ini dan semua scene berikutnya
                            for (let j = i; j <= maxScenes; j++) {
                                const currentSection = document.getElementById(`scene${j}-section`);
                                if (currentSection) {
                                    currentSection.classList.add('hidden');
                                    currentSection.querySelectorAll('input, select, textarea').forEach(el => {
                                        if (el.tagName === 'SELECT') el.selectedIndex = 0;
                                        else el.value = '';
                                        el.dispatchEvent(new Event('change'));
                                    });
                                }
                                const currentAddBtn = document.getElementById(`add-scene-btn-${j}`);
                                if (currentAddBtn && j > i) currentAddBtn.classList.add('hidden');
                            }
                            if (addBtn) addBtn.classList.remove('hidden');
                        });
                    }
                }
            }


            setupCharacterToggle('add-character-btn-2', 'remove-character-btn-2', 'character2-section');
            setupCharacterToggle('add-character-btn-3', 'remove-character-btn-3', 'character3-section');
            setupCharacterToggle('add-character-btn-4', 'remove-character-btn-4', 'character4-section');
            setupCharacterToggle('add-character-btn-5', 'remove-character-btn-5', 'character5-section');
            setupSceneToggles();
            
            // Fungsi untuk mendapatkan nilai final dari input (memeriksa opsi 'other')
            function getFinalValue(elementId) {
                const mainElement = document.getElementById(elementId);
                if (!mainElement) return '';
                if (mainElement.tagName.toLowerCase() === 'select' && mainElement.value === 'other') {
                    const otherElement = document.getElementById(elementId + '-other');
                    return otherElement ? otherElement.value.trim() : '';
                }
                return mainElement.value.trim();
            }

            // Fungsi untuk menambahkan data ke prompt
            function appendToPrompt(p, label, value) {
                return value ? `${p}${label}: ${value}\n` : p;
            }

            // Event listener untuk tombol generate
            document.getElementById('generate-btn').addEventListener('click', () => {
                let prompt = "Buatkan Video\n\n";

                prompt = appendToPrompt(prompt, "Jenis Video", getFinalValue("video-type"));
                prompt = appendToPrompt(prompt, "Nama Video", getFinalValue("video-name"));
                prompt += "\nPENTING: Pastikan suara karakter konsisten. Untuk dialog Bahasa Jawa, gunakan logat Jawa Timur yang natural dan jelas.\n";

                // --- BAGIAN KARAKTER ---
                prompt += "\n\n--- KARAKTER ---\n";
                let hasCharacters = false;
                for (let i = 1; i <= 5; i++) {
                    const section = document.getElementById(`character${i}-section`);
                    if (!section || section.classList.contains('hidden')) continue;
                    
                    const characterName = getFinalValue(`c${i}-name`);
                    if (!characterName) continue; // Lewati karakter jika tidak ada nama
                    
                    hasCharacters = true;
                    prompt += `\n--- KARAKTER ${i}: ${characterName.toUpperCase()} ---\n`;
                    
                    prompt += "[DETAIL FISIK]\n";
                    prompt = appendToPrompt(prompt, "Usia", getFinalValue(`c${i}-age`));
                    prompt = appendToPrompt(prompt, "Jenis Kelamin", getFinalValue(`c${i}-gender`));
                    prompt = appendToPrompt(prompt, "Etnis", getFinalValue(`c${i}-etnis`));
                    prompt = appendToPrompt(prompt, "Perawakan/Bentuk Tubuh", getFinalValue(`c${i}-body`));
                    prompt = appendToPrompt(prompt, "Warna Kulit", getFinalValue(`c${i}-skin`));
                    if (getFinalValue(`c${i}-gender`) === 'Perempuan') {
                       prompt = appendToPrompt(prompt, "Ukuran (Payudara)", getFinalValue(`c${i}-breasts`));
                    }
                    prompt = appendToPrompt(prompt, "Wajah", getFinalValue(`c${i}-face`));
                    prompt = appendToPrompt(prompt, "Rambut", getFinalValue(`c${i}-hair`));
                    prompt = appendToPrompt(prompt, "Pakaian Atas", getFinalValue(`c${i}-top`));
                    prompt = appendToPrompt(prompt, "Pakaian Bawah", getFinalValue(`c${i}-bottom`));
                    prompt = appendToPrompt(prompt, "Aksesori", getFinalValue(`c${i}-accessory`));
                    
                    prompt += "\n[SUARA]\n";
                    prompt = appendToPrompt(prompt, "Jenis Suara", getFinalValue(`c${i}-voice-type`));
                    prompt = appendToPrompt(prompt, "Cara Berbicara", getFinalValue(`c${i}-speech`));
                    prompt = appendToPrompt(prompt, "Aksen/Logat", getFinalValue(`c${i}-accent`));
                    prompt = appendToPrompt(prompt, "Deskripsi Suara", getFinalValue(`c${i}-voice-desc`));
                }
                if (!hasCharacters) {
                    prompt += "Tidak ada karakter yang didefinisikan.\n";
                }
                
                // --- PENGATURAN GLOBAL ---
                prompt += "\n\n--- PENGATURAN GLOBAL ---\n";
                prompt += "\n[LATAR TEMPAT & WAKTU]\n";
                prompt = appendToPrompt(prompt, "Desa", getFinalValue("global-village"));
                prompt = appendToPrompt(prompt, "Latar Tempat", getFinalValue("global-setting"));
                prompt = appendToPrompt(prompt, "Cuaca", getFinalValue("global-weather"));
                prompt = appendToPrompt(prompt, "Musim", getFinalValue("global-season"));
                prompt = appendToPrompt(prompt, "Waktu", getFinalValue("global-time"));
                prompt = appendToPrompt(prompt, "Jam", getFinalValue("global-clock"));

                prompt += "\n[DETAIL TEKNIS & VISUAL]\n";
                prompt = appendToPrompt(prompt, "Suasana Keseluruhan", getFinalValue("overall-mood"));
                prompt = appendToPrompt(prompt, "Suara Lingkungan / Ambiance", getFinalValue("ambience"));
                prompt = appendToPrompt(prompt, "Gaya Video/Art Style", getFinalValue("art-style"));
                prompt = appendToPrompt(prompt, "Kualitas Visual", getFinalValue("quality"));
                prompt = appendToPrompt(prompt, "Pencahayaan", getFinalValue("lighting"));
                prompt = appendToPrompt(prompt, "Sudut Kamera", getFinalValue("camera-angle"));
                prompt = appendToPrompt(prompt, "Gerakan Kamera", getFinalValue("camera-movement"));

                // --- BAGIAN SCENE ---
                prompt += "\n\n--- RUNTUTAN SCENE ---\n";
                for (let i = 1; i <= 6; i++) {
                    const section = document.getElementById(`scene${i}-section`);
                    if (!section || section.classList.contains('hidden')) continue;

                    prompt += `\n--- SCENE ${i} ---\n`;
                    
                    prompt += `[DETAIL ADEGAN]\n`;
                    prompt = appendToPrompt(prompt, "Karakter Terlibat", getFinalValue(`s${i}-characters`));
                    prompt = appendToPrompt(prompt, "Aksi Karakter", getFinalValue(`s${i}-action`));
                    prompt = appendToPrompt(prompt, "Ekspresi Karakter", getFinalValue(`s${i}-expression`));

                    const dialogLang = getFinalValue(`s${i}-dialog-lang`);
                    const dialogText = getFinalValue(`s${i}-dialog`);
                    
                    if (dialogText) {
                        prompt += `\n[DIALOG]\n`;
                        prompt = appendToPrompt(prompt, "Bahasa Dialog", dialogLang);
                        prompt += `Teks Dialog:\n${dialogText}\n`;
                    }
                }

                prompt += "\n\n--- NEGATIVE PROMPT ---\n";
                const negativeValue = getFinalValue('negative-prompt');
                if (negativeValue) {
                    prompt += `Hindari: ${negativeValue}\n`;
                }

                const outputContainer = document.getElementById('output-container');
                document.getElementById('prompt-output').value = prompt;
                outputContainer.classList.remove('hidden');
                outputContainer.scrollIntoView({ behavior: 'smooth' });
            });
            
            // Event listener untuk tombol salin
            document.getElementById('copy-btn').addEventListener('click', () => {
                const promptOutput = document.getElementById('prompt-output');
                promptOutput.select();
                document.execCommand('copy');
                const copyBtn = document.getElementById('copy-btn');
                copyBtn.textContent = 'Berhasil Disalin!';
                setTimeout(() => { copyBtn.textContent = 'Salin Teks Prompt'; }, 2000);
            });
        });
    </script>

</body>
</html>
