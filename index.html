<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>CHUKUM — Folha de Pagamento</title>
  <meta name="description" content="Planilha e gestão de folha de pagamento — CHUKUM" />
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    .container{max-width:1100px}
  </style>
</head>
<body class="bg-slate-50 text-slate-800 antialiased">
  <header class="bg-white shadow-sm">
    <div class="container mx-auto px-6 py-4 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-md bg-sky-600 flex items-center justify-center text-white font-bold">C</div>
        <div>
          <h1 class="text-lg font-semibold">CHUKUM</h1>
          <p class="text-xs text-slate-500">Ferramenta simples para gerar folha de pagamento</p>
        </div>
      </div>
      <nav class="text-sm text-slate-600 hidden md:flex gap-4">
        <a href="#tabela" class="hover:underline">Tabela</a>
        <a href="#exportar" class="hover:underline">Exportar</a>
      </nav>
    </div>
  </header>

  <main class="container mx-auto px-6 py-8">
    <section class="grid md:grid-cols-2 gap-8 items-start">
      <div class="bg-white p-6 rounded-lg shadow">
        <h2 class="text-2xl font-bold">Folha de Pagamento - CHUKUM</h2>
        <p class="mt-2 text-slate-600">Preencha os dados dos colaboradores e gere a folha com cálculos automáticos: horas extras, faltas proporcionais, descontos e salário líquido.</p>

        <div class="mt-6">
          <label class="block text-sm font-medium">Nome do colaborador</label>
          <input id="nome" class="mt-1 w-full px-3 py-2 border rounded" placeholder="Ex: João Silva" />

          <label class="block text-sm font-medium mt-3">Cargo</label>
          <input id="cargo" class="mt-1 w-full px-3 py-2 border rounded" placeholder="Ex: Técnico" />

          <label class="block text-sm font-medium mt-3">Data de admissão</label>
          <input id="admissao" type="date" class="mt-1 w-full px-3 py-2 border rounded" />

          <label class="block text-sm font-medium mt-3">Salário base (R$)</label>
          <input id="salario" type="number" step="0.01" class="mt-1 w-full px-3 py-2 border rounded" placeholder="0.00" />

          <label class="block text-sm font-medium mt-3">Horas extras (horas)</label>
          <input id="horasExtra" type="number" step="0.01" class="mt-1 w-full px-3 py-2 border rounded" placeholder="Horas extras" />

          <label class="block text-sm font-medium mt-3">Horista (R$ por hora — opcional)</label>
          <input id="horista" type="number" step="0.01" class="mt-1 w-full px-3 py-2 border rounded" placeholder="Valor hora" />

          <label class="block text-sm font-medium mt-3">Faltas / Dias</label>
          <input id="faltas" type="number" step="1" class="mt-1 w-full px-3 py-2 border rounded" placeholder="Número de dias" />

          <label class="block text-sm font-medium mt-3">Desconto Sindicato (R$)</label>
          <input id="sindicato" type="number" step="0.01" class="mt-1 w-full px-3 py-2 border rounded" placeholder="0.00" />

          <label class="block text-sm font-medium mt-3">Desconto Vale Transporte (R$)</label>
          <input id="vt" type="number" step="0.01" class="mt-1 w-full px-3 py-2 border rounded" placeholder="0.00" />

          <label class="block text-sm font-medium mt-3">Outros descontos (R$)</label>
          <input id="outros" type="number" step="0.01" class="mt-1 w-full px-3 py-2 border rounded" placeholder="0.00" />

          <div class="flex gap-2 mt-4">
            <button id="adicionar" class="bg-sky-600 text-white px-4 py-2 rounded">Adicionar à tabela</button>
            <button id="limpar" class="border px-4 py-2 rounded">Limpar</button>
          </div>

          <p class="text-xs text-slate-400 mt-3">As fórmulas aplicadas: hora extra = (salário / 220) * 1.5 * horasExtra; desconto faltas = (salário / 30) * faltas.</p>
        </div>
      </div>

      <div class="bg-white p-6 rounded-lg shadow">
        <h3 class="text-xl font-semibold">Resumo rápido</h3>
        <div class="mt-4 space-y-2 text-sm text-slate-600">
          <div>Preencha e clique em <strong>Adicionar à tabela</strong> para gerar as linhas.</div>
          <div>Você pode exportar a tabela como CSV para abrir no Excel.</div>
        </div>

        <div id="exportar" class="mt-6 flex gap-2">
          <button id="exportCsv" class="bg-green-600 text-white px-4 py-2 rounded">Exportar CSV</button>
          <button id="exportJson" class="border px-4 py-2 rounded">Exportar JSON</button>
          <button id="downloadXlsx" class="border px-4 py-2 rounded">Baixar Excel (gerado no navegador)</button>
        </div>

        <div class="mt-6 text-sm text-slate-500">Observação: valores e fórmulas são um modelo — revise conforme a legislação local e holerites da sua empresa.</div>
      </div>
    </section>

    <section id="tabela" class="mt-8 bg-white p-6 rounded-lg shadow">
      <h3 class="text-lg font-semibold">Tabela da Folha</h3>
      <div class="overflow-x-auto mt-4">
        <table id="sheetTable" class="min-w-full table-auto text-sm">
          <thead>
            <tr class="bg-slate-100 text-left">
              <th class="px-3 py-2">Nome</th>
              <th class="px-3 py-2">Cargo</th>
              <th class="px-3 py-2">Data Admissão</th>
              <th class="px-3 py-2">Salário Base</th>
              <th class="px-3 py-2">Horas Extras (R$)</th>
              <th class="px-3 py-2">Horista (R$)</th>
              <th class="px-3 py-2">Descontos</th>
              <th class="px-3 py-2">Faltas/Dias</th>
              <th class="px-3 py-2">Total Descontos</th>
              <th class="px-3 py-2">Salário Líquido</th>
              <th class="px-3 py-2">Ações</th>
            </tr>
          </thead>
          <tbody id="tbody"></tbody>
        </table>
      </div>
    </section>

    <footer class="mt-8 text-sm text-slate-500">© CHUKUM — Folha de Pagamento</footer>
  </main>

  <script>
    // Utilitários
    function formatMoney(v){return Number(v).toLocaleString('pt-BR',{minimumFractionDigits:2,maximumFractionDigits:2})}

    const tbody = document.getElementById('tbody');
    const adicionar = document.getElementById('adicionar');
    const limpar = document.getElementById('limpar');

    function calcula(salario, horasExtra, horista, faltas, sindicato, vt, outros){
      salario = Number(salario) || 0;
      horasExtra = Number(horasExtra) || 0;
      horista = Number(horista) || 0;
      faltas = Number(faltas) || 0;
      sindicato = Number(sindicato) || 0;
      vt = Number(vt) || 0;
      outros = Number(outros) || 0;

      // Base: considerar 220 horas mensais padrão
      const valorHora = salario / 220;
      // Hora extra com 50% adicional (1.5x)
      const valorHorasExtra = (valorHora * 1.5) * horasExtra;
      // Se informado horista, considerar como adicional (valor em R$ já)
      const valorHorista = horista || 0;
      // Desconto por faltas proporcional (salario/30 * dias)
      const descontoFaltas = (salario / 30) * faltas;

      const totalDescontos = Number(sindicato) + Number(vt) + Number(outros) + descontoFaltas;
      const bruto = salario + valorHorasExtra + valorHorista;
      const liquido = bruto - totalDescontos;

      return {
        valorHorasExtra, valorHorista, descontoFaltas, totalDescontos, bruto, liquido
      }
    }

    function criaLinha(data){
      const tr = document.createElement('tr');
      tr.className = 'border-t';
      tr.innerHTML = `
        <td class="px-3 py-2">${data.nome}</td>
        <td class="px-3 py-2">${data.cargo}</td>
        <td class="px-3 py-2">${data.admissao}</td>
        <td class="px-3 py-2">R$ ${formatMoney(data.salario)}</td>
        <td class="px-3 py-2">R$ ${formatMoney(data.valorHorasExtra)}</td>
        <td class="px-3 py-2">R$ ${formatMoney(data.valorHorista)}</td>
        <td class="px-3 py-2">R$ ${formatMoney(data.totalDescontos)}</td>
        <td class="px-3 py-2">${data.faltas}</td>
        <td class="px-3 py-2">R$ ${formatMoney(data.totalDescontos)}</td>
        <td class="px-3 py-2">R$ ${formatMoney(data.liquido)}</td>
        <td class="px-3 py-2"><button class="text-sm text-red-600 deleteBtn">Remover</button></td>
      `;
      return tr;
    }

    adicionar.addEventListener('click', function(e){
      e.preventDefault();
      const nome = document.getElementById('nome').value.trim();
      if(!nome){alert('Preencha o nome do colaborador');return}
      const cargo = document.getElementById('cargo').value.trim();
      const admissao = document.getElementById('admissao').value;
      const salario = Number(document.getElementById('salario').value) || 0;
      const horasExtra = Number(document.getElementById('horasExtra').value) || 0;
      const horista = Number(document.getElementById('horista').value) || 0;
      const faltas = Number(document.getElementById('faltas').value) || 0;
      const sindicato = Number(document.getElementById('sindicato').value) || 0;
      const vt = Number(document.getElementById('vt').value) || 0;
      const outros = Number(document.getElementById('outros').value) || 0;

      const c = calcula(salario, horasExtra, horista, faltas, sindicato, vt, outros);
      const obj = {
        nome, cargo, admissao, salario, faltas,
        valorHorasExtra: c.valorHorasExtra,
        valorHorista: c.valorHorista,
        descontoFaltas: c.descontoFaltas,
        totalDescontos: c.totalDescontos,
        liquido: c.liquido
      };

      const tr = criaLinha(obj);
      tbody.appendChild(tr);

      // limpa campos
      document.getElementById('nome').value='';
      document.getElementById('cargo').value='';
      document.getElementById('admissao').value='';
      document.getElementById('salario').value='';
      document.getElementById('horasExtra').value='';
      document.getElementById('horista').value='';
      document.getElementById('faltas').value='';
      document.getElementById('sindicato').value='';
      document.getElementById('vt').value='';
      document.getElementById('outros').value='';
    });

    limpar.addEventListener('click', function(){
      document.getElementById('nome').value='';
      document.getElementById('cargo').value='';
      document.getElementById('admissao').value='';
      document.getElementById('salario').value='';
      document.getElementById('horasExtra').value='';
      document.getElementById('horista').value='';
      document.getElementById('faltas').value='';
      document.getElementById('sindicato').value='';
      document.getElementById('vt').value='';
      document.getElementById('outros').value='';
    });

    // Delegação para remover
    tbody.addEventListener('click', function(e){
      if(e.target.classList.contains('deleteBtn')){
        e.target.closest('tr').remove();
      }
    });

    // Exportar CSV
    function tableToCSV(){
      const rows = [];
      const headers = ['Nome','Cargo','Data de admissão','Salário Base','Horas Extras (R$)','Horista (R$)','Descontos (R$)','Faltas/Dias','Total Descontos (R$)','Salário Líquido (R$)'];
      rows.push(headers.join(','));
      document.querySelectorAll('#tbody tr').forEach(tr=>{
        const cols = Array.from(tr.querySelectorAll('td')).slice(0,10).map(td=>td.innerText.replace(/\s+/g,' '));
        rows.push(cols.map(c=>'"'+c.replace(/"/g,'""')+'"').join(','));
      });
      return rows.join('\n');
    }

    document.getElementById('exportCsv').addEventListener('click', function(){
      const csv = tableToCSV();
      const blob = new Blob([csv], {type: 'text/csv;charset=utf-8;'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = 'folha_chukum.csv';
      a.click();
      URL.revokeObjectURL(url);
    });

    document.getElementById('exportJson').addEventListener('click', function(){
      const data = [];
      document.querySelectorAll('#tbody tr').forEach(tr=>{
        const tds = tr.querySelectorAll('td');
        data.push({
          nome: tds[0].innerText,
          cargo: tds[1].innerText,
          admissao: tds[2].innerText,
          salario_base: tds[3].innerText,
          horas_extras: tds[4].innerText,
          horista: tds[5].innerText,
          descontos: tds[6].innerText,
          faltas: tds[7].innerText,
          total_descontos: tds[8].innerText,
          salario_liquido: tds[9].innerText
        });
      });
      const blob = new Blob([JSON.stringify(data, null, 2)], {type: 'application/json'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url; a.download = 'folha_chukum.json'; a.click(); URL.revokeObjectURL(url);
    });

    // Gerar arquivo Excel simples no navegador (xlsx) usando SheetJS if available
    document.getElementById('downloadXlsx').addEventListener('click', async function(){
      if(typeof XLSX === 'undefined'){
        // carrega SheetJS CDN
        const script = document.createElement('script');
        script.src = 'https://cdn.sheetjs.com/xlsx-latest/package/dist/xlsx.full.min.js';
        document.head.appendChild(script);
        script.onload = ()=>generateXlsx();
      } else generateXlsx();
    });

    function generateXlsx(){
      const ws_data = [];
      const headers = ['Nome','Cargo','Data de admissão','Salário Base','Horas Extras (R$)','Horista (R$)','Descontos (R$)','Faltas/Dias','Total Descontos (R$)','Salário Líquido (R$)'];
      ws_data.push(headers);
      document.querySelectorAll('#tbody tr').forEach(tr=>{
        const cols = Array.from(tr.querySelectorAll('td')).slice(0,10).map(td=>td.innerText.replace(/R\$ /g,'').replace(/\./g,','));
        ws_data.push(cols);
      });
      const wb = XLSX.utils.book_new();
      const ws = XLSX.utils.aoa_to_sheet(ws_data);
      XLSX.utils.book_append_sheet(wb, ws, 'Folha');
      XLSX.writeFile(wb, 'folha_chukum.xlsx');
    }

  </script>
</body>
</html>
