<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Ficha de Movimentação de Membros</title>
  <style>
    /* Estilo geral */
    body { font-family: "Segoe UI", Arial, sans-serif; margin: 0; padding: 0; background: #f0f2f5; }
    h2 { text-align: center; padding: 20px; background: #2c3e50; color: white; margin: 0; border-bottom: 4px solid #27ae60; }
    form { background: #fff; padding: 30px; border-radius: 12px; max-width: 1000px; margin: 30px auto; box-shadow: 0 6px 20px rgba(0,0,0,0.15); }
    fieldset { margin-bottom: 25px; border: 1px solid #ddd; border-radius: 10px; padding: 20px; }
    legend { font-weight: bold; color: #2c3e50; padding: 0 8px; }
    label { display: block; margin-top: 12px; font-size: 14px; color: #333; }
    input, select, textarea { width: 100%; padding: 10px; margin-top: 6px; border: 1px solid #ccc; border-radius: 6px; font-size: 14px; transition: border 0.3s ease; }
    input:focus, select:focus, textarea:focus { border-color: #27ae60; outline: none; }
    .inline { display: flex; gap: 15px; }
    .inline label { flex: 1; }
    .foto { text-align: right; margin-bottom: 20px; }
    .foto div { border: 2px dashed #aaa; width: 120px; height: 150px; text-align: center; line-height: 150px; margin-left: auto; font-size: 12px; color: #777; border-radius: 6px; }
    button { background: #27ae60; color: white; padding: 14px 28px; border: none; border-radius: 8px; cursor: pointer; font-size: 16px; display: block; margin: auto; transition: background 0.3s ease, transform 0.2s ease; }
    button:hover { background: #219150; transform: scale(1.05); }
    textarea { resize: vertical; }
  </style>
</head>
<body>
  <h2>📋 Ficha de Movimentação de Membros</h2>
  
  <form action="https://formspree.io/f/xzzayogn" method="POST">
    <div class="foto">
      <div>FOTO 3x4</div>
    </div>

    <fieldset>
      <legend>Tipo de Movimentação</legend>
      <div class="inline">
        <label><input type="checkbox" name="admissao"> Admissão</label>
        <label><input type="checkbox" name="registro_interno"> Registro Interno (RI)</label>
        <label><input type="checkbox" name="batismo"> Batismo</label>
      </div>
      <div class="inline">
        <label><input type="checkbox" name="recadastramento"> Recadastramento</label>
        <label><input type="checkbox" name="transferencia"> Transferência</label>
        <label><input type="checkbox" name="reconciliacao"> Reconciliação</label>
      </div>
      <div class="inline">
        <label><input type="checkbox" name="disciplina"> Disciplina</label>
        <label><input type="checkbox" name="desligamento"> Desligamento</label>
      </div>
    </fieldset>

    <fieldset>
      <legend>Dados Pessoais</legend>
      <label>Nome: <input type="text" name="nome"></label>
      <div class="inline">
        <label>Cargo: <input type="text" name="cargo"></label>
        <label>Data Consagração: <input type="date" name="data_consagracao"></label>
      </div>
      <div class="inline">
        <label>Congregação: <input type="text" name="congregacao"></label>
        <label>Setor: <input type="text" name="setor"></label>
        <label>Regional: <input type="text" name="regional"></label>
      </div>
      <div class="inline">
        <label>Pai: <input type="text" name="pai"></label>
        <label>Mãe: <input type="text" name="mae"></label>
      </div>
      <div class="inline">
        <label>Data Nasc.: <input type="date" name="data_nascimento"></label>
        <label>Natural de: <input type="text" name="natural_de"></label>
        <label>UF: <input type="text" name="uf_nasc"></label>
      </div>
      <div class="inline">
        <label>Nacionalidade: <input type="text" name="nacionalidade"></label>
        <label>Sexo: <select name="sexo">
          <option>Masculino</option>
          <option>Feminino</option>
        </select></label>
      </div>
      <label>Endereço: <input type="text" name="endereco"></label>
      <div class="inline">
        <label>Bairro: <input type="text" name="bairro"></label>
        <label>Cidade: <input type="text" name="cidade"></label>
        <label>UF: <input type="text" name="uf_endereco"></label>
        <label>CEP: <input type="text" name="cep"></label>
      </div>
      <div class="inline">
        <label>Fone Res.: <input type="text" name="fone_res"></label>
        <label>Fone Cel.: <input type="text" name="fone_cel"></label>
        <label>Fone Com.: <input type="text" name="fone_com"></label>
      </div>
      <label>E-mail: <input type="email" name="email"></label>
      <label>Facebook: <input type="text" name="facebook"></label>
      <div class="inline">
        <label>Est. Civil: <input type="text" name="estado_civil"></label>
        <label>Data Casamento: <input type="date" name="data_casamento"></label>
        <label>Profissão: <input type="text" name="profissao"></label>
      </div>
      <div class="inline">
        <label>CPF: <input type="text" name="cpf"></label>
        <label>RG: <input type="text" name="rg"></label>
        <label>Data Exp.: <input type="date" name="data_exp_rg"></label>
        <label>UF RG: <input type="text" name="uf_rg"></label>
      </div>
      <div class="inline">
        <label>Título Eleitor: <input type="text" name="titulo_eleitor"></label>
        <label>Zona: <input type="text" name="zona"></label>
        <label>Seção: <input type="text" name="secao"></label>
      </div>
      <div class="inline">
        <label>Escolaridade: <input type="text" name="escolaridade"></label>
        <label>Tipo Sanguíneo: <input type="text" name="tipo_sanguineo"></label>
      </div>
    </fieldset>

    <fieldset>
      <legend>Dados Ministeriais</legend>
      <div class="inline">
        <label>Batizado c/ Espírito Santo: <select name="batizado_espirito">
          <option>Sim</option>
          <option>Não</option>
        </select></label>
        <label>Data: <input type="date" name="data_batizado_espirito"></label>
      </div>
      <div class="inline">
        <label>Data Batismo: <input type="date" name="data_batismo"></label>
        <label>Igreja: <input type="text" name="igreja_batismo"></label>
        <label>Cidade: <input type="text" name="cidade_batismo"></label>
        <label>UF: <input type="text" name="uf_batismo"></label>
      </div>
      <div class="inline">
        <label>Data Admissão: <input type="date" name="data_admissao"></label>
        <label>Data Conversão: <input type="date" name="data_conversao"></label>
      </div>
      <label>Local da Conversão: <input type="text" name="local_conversao"></label>
      <label>Veio com Carta? <select name="veio_com_carta">
        <option>Sim</option>
        <option>Não</option>
      </select></label>
      <div class="inline">
        <label>Igreja de Origem: <input type="text" name="igreja_origem"></label>
        <label>Cidade: <input type="text" name="cidade_origem"></label>
        <label>UF: <input type="text" name="uf_origem"></label>
      </div>
    </fieldset>

    <fieldset>
      <legend>Família</legend>
      <label>Nome do Cônjuge: <input type="text" name="conjuge"></label>
      <label>Quant. Filhos: <input type="number" name="quant_filhos"></label>
      <textarea name="detalhes_filhos" rows="4" placeholder="Nome, Data Nascimento, Evang./Não Evang."></textarea>
    </fieldset>

    <fieldset>
      <legend>Observações</legend>
      <textarea name="observacoes" rows="4" placeholder="Digite observações aqui..."></textarea>
    </fieldset>

    <button type="submit">✅ Enviar Cadastro</button>
  </form>
</body>
</html>
